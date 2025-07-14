

- SMS and Call Reporting
- ILMessageFilterSubAction
-  ILMessageFilterSubAction.none 

Case

# ILMessageFilterSubAction.none

Allows the system to show the message unfiltered due to insufficient information to determine an action.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
case none
```

## Discussion

In a query response, setting this value allows the system to show the message unfiltered.

## See Also

### Transactional Subactions

case transactionalOthers

Prevents the system from showing the message normally, filtered as an Others message.

case transactionalFinance

Prevents the system from showing the message normally, filtered as a Finance message.

case transactionalOrders

Prevents the system from showing the message normally, filtered as an Orders (eCommerce) message.

case transactionalReminders

Prevents the system from showing the message normally, filtered as a Reminder message.

case transactionalHealth

Prevents the system from showing the message normally, filtered as a Health message.

case transactionalWeather

Prevents the system from showing the message normally, filtered as a Weather message.

case transactionalCarrier

Prevents the system from showing the message normally, filtered as a Carrier message.

case transactionalRewards

Prevents the system from showing the message normally, filtered as a Rewards message.

case transactionalPublicServices

Prevents the system from showing the message normally, filtered as a Government message.

