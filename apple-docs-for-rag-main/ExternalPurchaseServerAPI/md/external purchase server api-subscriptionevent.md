

- External Purchase Server API
-  subscriptionEvent 

Type

# subscriptionEvent

The event in the subscription’s life cycle that the transaction represents.

External Purchase Server API 1.0.0+

``` source
string subscriptionEvent
```

## Possible Values 

`SUBSCRIPTION_START`  

`RENEWAL`  

`SUBSCRIPTION_CHANGE`  

`SUBSCRIPTION_PAYMENT`  

## Mentioned in 

Reporting tokens with transactions

## Discussion

Allowed values: `SUBSCRIPTION_START`, `RENEWAL`, `SUBSCRIPTION_CHANGE`, `SUBSCRIPTION_PAYMENT`

Use the allowed values to indicate the subscription event in a SubscriptionBuyLineItem, as follows:

`SUBSCRIPTION_START`  
The first time you report the subscription, for example, when a customer first subscribes.

`RENEWAL`  
A subscription renewal.

`SUBSCRIPTION_CHANGE`  
The customer upgraded or downgraded the subscription. An *upgrade* is a change to the subscription that adds features or functionality, or increases the subscription renewal period (such as from a weekly to a monthly renewal). A *downgrade* is a change to the subscription that reduces features or functionality, or decreases the subscription period (such as from an annual to a monthly renewal).

`SUBSCRIPTION_PAYMENT`  
A payment for the subscription.

## See Also

### Supplying subscription info

type subscriptionDaysOfPaidService

The total number of days of paid service for the subscription.

type subscriptionEndDate

The UNIX date, in milli-seconds, the subscription renewal cycle ends.

type subscriptionStartDate

The UNIX date, in milli-seconds, of the start of the subscription renewal period.

type referenceLineItemId

The line item identifier of another transaction, that the report references.

