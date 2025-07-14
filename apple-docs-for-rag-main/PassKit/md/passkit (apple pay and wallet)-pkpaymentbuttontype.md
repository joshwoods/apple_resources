

- PassKit (Apple Pay and Wallet)
-  PKPaymentButtonType 

Enumeration

# PKPaymentButtonType

The Apple Pay button types you can display to initiate Apple Pay transactions.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
enum PKPaymentButtonType
```

## Overview

The button type you use for payments made with Apple Pay can affect the purchasing experience. Choose a button type that best fits with the terminology and flow of your purchase or payment experience. For design guidance, see Human Interface Guidelines > Apple Pay > Buttons and Marks.

Before using a specific button type, check that it’s available to the iOS version that your app is running on. Create buttons using the buttonWithType:style: method.

## Topics

### Payment button types

case plain

An Apple Pay button with the Apple Pay logo only, useful when an additional call to action isn’t needed.

case buy

An Apple Pay button useful for product purchases.

case addMoney

An Apple Pay button useful for adding money to a card, account, or payment system.

case book

An Apple Pay button useful for booking trips, flights, or other experiences.

case checkout

An Apple Pay button useful for purchase experiences that include other payment buttons that start with “Check out”.

case `continue`

An Apple Pay button useful for general purchases.

case contribute

An Apple Pay button useful to help people contribute money to projects, causes, organizations, and other entities.

case donate

An Apple Pay button used by approved nonprofit organization that lets people make donations.

case inStore

An Apple Pay button useful for paying bills or invoices.

case order

An Apple Pay button useful for placing orders for such as like meals or flowers.

case reload

An Apple Pay button useful for adding money to a card, account, or payment system.

case rent

An Apple Pay button useful for renting items such as cars or scooters.

case setUp

An Apple Pay button useful for prompting the user to set up a card.

case subscribe

An Apple Pay button useful for purchasing a subscription such as a gym membership or meal-kit delivery service.

case support

An Apple Pay button useful supporting people give money to projects, causes, organizations, and other entities.

case tip

An Apple Pay button useful useful for letting people tip for goods or services.

case topUp

An Apple Pay button useful for adding money to a card, account, or payment system.

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

### Configuring the appearance

enum PKPaymentButtonStyle

A type that indicates the available appearances for an Apple Pay button.

var cornerRadius: CGFloat

The radius, in points, for the rounded corners on the button.

