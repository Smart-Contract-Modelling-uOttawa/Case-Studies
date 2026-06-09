# Pizza Delivery Contract
## Contract Text
Pizza delivery contract: 
- The customer orders a pizza from a restaurant to be delivered within 30 minutes; 
- The customer agrees to pay the price of the pizza upon delivery; iii) If delivery is late, the customer has the option (power) to cancel the contract or pay half the price upon delivery.
## Note
This specification does not capture the expectations of the customer; if the pizza is delivered late and the customer chooses the `pay late' option, then she must pay both the regular price \textit{and} the half price for the pizza! To fix the problem, \symboleoc{Opay} needs to be amended into \symboleoc{Opay: Obligation(cust, restaurant, happens(delivered, t) and t before ordered.Time + 30min, happensBefore(paid, t + 5min))}.
With this amendment, \symboleoc{Opay} becomes active and obliges the customer to pay for the pizza the regular price only if delivered on time. This example underscores the importance of formal analysis of Symboleo specifications to ensure they are consistent with the expectations of contracting parties.
