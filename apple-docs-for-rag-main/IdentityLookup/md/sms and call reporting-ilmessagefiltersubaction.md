

- SMS and Call Reporting
-  ILMessageFilterSubAction 

Enumeration

# ILMessageFilterSubAction

Responds to a received message with a filter subaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum ILMessageFilterSubAction
```

## Topics

### Transactional Subactions

case none

Allows the system to show the message unfiltered due to insufficient information to determine an action.

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

### Promotional Subactions

case promotionalOthers

Prevents the system from showing the message normally, filtered as an Others message.

case promotionalOffers

Prevents the system from showing the message normally, filtered as an Offers message.

case promotionalCoupons

Prevents the system from showing the message normally, filtered as an Coupons message.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Responses

class ILMessageFilterCapabilitiesQueryResponse

A response to a message filter capabilities query request.

