

- PassKit (Apple Pay and Wallet)
- PKPaymentButtonType
-  PKPaymentButtonType.setUp 

Case

# PKPaymentButtonType.setUp

An Apple Pay button useful for prompting the user to set up a card.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
case setUp
```

## Discussion

This button looks like:

You can display this button when the device and parental controls support Apple Pay but the user has not yet added a card. Use the PKPaymentAuthorizationViewController class’s canMakePayments() method to determine whether the device supports Apple Pay. If canMakePayments() returns true, call canMakePayments(usingNetworks:capabilities:) to determine whether the user has added any cards.

As soon as the user taps this button, initiate the process of setting up a new card (for example, by calling the openPaymentSetup() method).

For design guidance, see Human Interface Guidelines > Apple Pay > Buttons and Marks.

## See Also

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

case subscribe

An Apple Pay button useful for purchasing a subscription such as a gym membership or meal-kit delivery service.

case support

An Apple Pay button useful supporting people give money to projects, causes, organizations, and other entities.

case tip

An Apple Pay button useful useful for letting people tip for goods or services.

