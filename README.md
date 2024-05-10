# Hotel-booking-prediction
In the competitive hotel industry, offering flexible cancellation policies can be a double-edged sword. While allowing clients to cancel bookings up until the last minute can attract more customers, it also leads to a high cancellation rate.

## Business problem ##
How can a hotel maximize its revenue by optimally managing overbookings, considering the
risks and costs involved?

## The Challenge ## 
You are tasked with developing a comprehensive strategy to determine the ideal overbooking
rate for a hotel that allows cancellations until the last minute. This involves creating predictive
models to balance the benefit of filling as many rooms as possible against the risk of having to
compensate guests when overbooking leads to more guests than available rooms.

## Assumptions ##
Seasonality effects on booking rates are not considered.  
The demand is consistently strong, allowing for 100% booking of available rooms.

## PROPOSED SOLUTION ##
The solution proposed here is to define an overbooking rate for each customer type. This strategy involves analyzing customer behavior, optimizing revenue through tailored overbooking strategies, and minimizing losses by recognizing cancellation tendencies. The solution is defined as a data-driven overbooking model involves using machine learning techniques to predict the "no-show" probability (cancellation rate) of each customer. This personal information is then utilized to determine the best overbooking limits, with the goal of maximizing expected revenue. 

One simple definition for the overbooking rate is to set it equal to the cancellation rate. This definition implies for the solution proposed that the rate at which reservations are canceled by a customer type is used as a proxy for determining the overbooking rate for this customer type. This could mean that a business or service provider may intentionally accept more reservations for customer type with highter cancellation rates or put them intentionally in waiting lists despite of beeing available rooms assuming certain cancellation pattern. 

In conclusion,  different customer types may require distinct overbooking strategies. By identifying these customer types, hotels can develop optimal overbooking strategies that balance revenue maximization with customer satisfaction, ensuring that overbooking practices align with the needs and behaviors of specific customer segments.

This solution is based on two Classification problems:
1. Identifying type of customer: How characteristics extracted from the booking information of a customer can be asigned to a customer type?
2. Identifying the probability that the customer type will be cancelling the booking or not.
3. Calculate overbooking limit (excess demand over capacity) for each customer type. 
4. Calculate Reveneu as the sum of the reveneu per customer type.


According to the problem conditions, price changes over time will not be considered

**Bibliography:**
    
Varini, Kate. (2011). The Impact of Overbooking on Customer Loyalty: Can it be Positive?

Overbooking Strategy: Right on Target or a Shot in the (Hotel’s) Foot?
url: https://asksuite.com/blog/overbooking-strategy-good-practices/

¿Cómo influye el overbooking en los ingresos de los hoteles?
url: https://www.yieldplanet.com/es/how-does-overbooking-influence-hotel-revenue/

