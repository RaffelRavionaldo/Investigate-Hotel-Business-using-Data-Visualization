# Investigate-Hotel-Business-using-Data-Visualization
mini project from rakamin data science bootcamp, Here I am doing an investigation on hotel booking data

## Data Processing

### Overcoming Null Data

![image](https://user-images.githubusercontent.com/94748637/212446510-d6cf3efa-daa9-4240-a74d-cfb0277b287e.png)

From the table above, we know that data have a null value in 4 columns. For children we can fill with 0 because we assume that customers don’t have a child and for agent we fill with 0 because I think customer place an order without an agent. For null data in the city we fill it with mode at city column.

here is the syntax for doing it :

![image](https://user-images.githubusercontent.com/94748637/212446532-9be90000-d71c-4306-a4c2-bba1b930562c.png)

### Change Value at Meal column

![image](https://user-images.githubusercontent.com/94748637/212446549-d6cdfc76-0dcf-4757-8746-83db71466def.png)

From the picture above, we know at meal column have values that have the same meaning, it’s Undefined and No Meal, so we can changes Undefined to be No Meal.

here is the syntax for doing it :

![image](https://user-images.githubusercontent.com/94748637/212446568-11dc61c1-b9ef-4a6f-9ca9-2a2220ff856c.png)

### Discard Unnecessary Data : : Remove data that have an unreasonable total customer![image](https://user-images.githubusercontent.com/94748637/212446585-5e74a4d4-1158-4d32-b637-89d743fbdc29.png)

![image](https://user-images.githubusercontent.com/94748637/212446589-5b47ff8c-b5f6-4ee6-9742-56dc7e2ae846.png)

We can see that we have an outlier in the total number of guests data, but it's not problem because sometimes a customer do the hotel booking for his big family /company/etc, and we have ambigious data, there is data that dont have adults on hotel bookings and we must check is there any booking that have 0 customer or no.

how to do it :

![image](https://user-images.githubusercontent.com/94748637/212446604-86bf3dfe-cf61-406e-838d-87edf543ca11.png)

### Discard Unnecessary Data : Remove data that have stay duration = 0

Sometimes the customer/system makes an error where the column for the number of days to stay Is not filled/not obtained. So it will have a value of 0 and the data must be deleted.

Here is the syntax for doing it : 

![image](https://user-images.githubusercontent.com/94748637/212446632-6c2ea2e0-355d-42c8-a0bb-cee8c1b32570.png)

## Monthly Hotel Booking Analysis Based on Hotel Type

![image](https://user-images.githubusercontent.com/94748637/212446641-295db790-3ead-4887-8805-078a3274e510.png)

From the graph above, we know that :

1. The months with the highest number of hotel bookings are June, July and August because it is when school and college students are on semester break and during the dry season. So it’s perfect for going on vacation.

2. The months with the lowest number of hotel bookings are January, February and March. This can happen because is the start of the year where there are usually no long holidays.

3. At the end of the year, The number of hotel bookings has increased, but not as much as the top months, this can be happen because it’s the rainy season in that month and usually the price of necessities increases, we can increase the number of hotel bookings by making end year promos in collaboration with tourism.

4.We should make promos and advertise in May because the following month is the top month so it’s hoped that the number of hotel booking will increase and at the end of the year a tour package will be made that seems chepaer .

## Impact Analysis of Stay Duration on Hotel Booking Cancellation Rates

![image](https://user-images.githubusercontent.com/94748637/212446692-e268372d-c318-45df-959a-2f05e9b50553.png)

From the graph above, we know that :

1. City Hotel have a higher cancellation rate than a resort hotel.

2. At city hotel, when the duration of stay is longer, the cancellation rate will be higher.

3. Resort hotel have low cancellation rate, the highest cancellation rate is when the duration of stay is 3-4 weeks, is about 35%.

4. For reduce cancellation rate at city hotel, we can make a promo that’s such as the longer customer stay the cheaper the rental of hotel’s room price per night.

## Impact Analysis of Lead Time on Hotel Bookings Cancellation Rate

![image](https://user-images.githubusercontent.com/94748637/212446733-79c76725-3cda-4535-994e-e3eadde0fdc8.png)

From the graph above, we know that :

1. At Resort hotel, at 1-2 months and 3-4 months has a higher cancellation rate than others lead time. To overcome this, we have to make a deposit system so that the hotel doesn’t lose too much if the booking is cancelled.

2. At city hotel, at 5-6 months and 7-8 months has a higher cancellation rate than others lead time. To overcome this, we can provide discounts on other services such as discount on food and other hotel services (spa, gym, swimming pool etc).
