

- Apple Pay on the Web
-  ApplePayButtonType 

Enumeration

# ApplePayButtonType

A type that indicates the button types that you can display to initiate Apple Pay transactions.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
enum ApplePayButtonType
```

## Overview

The values for the button type:

`"add-money"`  
An Apple Pay button useful for adding money to a card, account, or payment system.

For more information, see PKPaymentButtonType.addMoney.

`"book"`  
An Apple Pay button useful for booking trips, flights, or other experiences.

For more information, see PKPaymentButtonType.book.

`"buy"`  
An Apple Pay button useful for product purchases.

For more information, see PKPaymentButtonType.buy.

`"check-out"`  
An Apple Pay button useful for purchase experiences that include other payment buttons that start with “Check out.”

For more information, see PKPaymentButtonType.checkout.

`"continue"`  
An Apple Pay button useful for general purchases.

For more information, see PKPaymentButtonType.continue.

`"contribute"`  
An Apple Pay button useful to help people contribute money to projects, causes, organizations, and other entities.

For more information, see PKPaymentButtonType.contribute.

`"donate"`  
An Apple Pay button used by approved nonprofit organization that lets people make donations.

For more information, see PKPaymentButtonType.donate.

`"order"`  
An Apple Pay button useful for placing orders for items such as meals or flowers.

For more information, see PKPaymentButtonType.order.

`"pay"`  
An Apple Pay button useful for paying bills or invoices.

For more information, see PKPaymentButtonType.inStore.

`"plain"`  
An Apple Pay button with the Apple Pay logo only, useful when an additional call to action isn’t needed.

For more information, see PKPaymentButtonType.plain.

`"reload"`  
An Apple Pay button useful for adding money to a card, account, or payment system.

For more information, see PKPaymentButtonType.reload.

`"rent"`  
An Apple Pay button useful for renting items such as cars or scooters.

For more information, see PKPaymentButtonType.rent.

`"set-up"`  
An Apple Pay button useful for prompting the user to set up a card.

For more information, see PKPaymentButtonType.setUp.

`"subscribe"`  
An Apple Pay button useful for purchasing a subscription such as a gym membership or meal-kit delivery service.

For more information, see PKPaymentButtonType.subscribe.

`"support"`  
An Apple Pay button useful for helping people give money to projects, causes, organizations, and other entities.

For more information, see PKPaymentButtonType.support.

`"tip"`  
An Apple Pay button useful for letting people tip for goods or services.

For more information, see PKPaymentButtonType.tip.

`"top-up"`  
An Apple Pay button useful for adding money to a card, account, or payment system.

For more information, see PKPaymentButtonType.topUp.

## Topics

### Enumeration Cases

add

book

buy

check

continue

contribute

donate

order

pay

plain

reload

rent

set

subscribe

support

tip

top

## See Also

### Configuring appearance

type

The kind of Apple Pay button, such as a button for purchasing a subscription.

buttonstyle

The appearance of the Apple Pay button, such as a black button with white lettering.

locale

The language and region used for the displayed Apple Pay button.

ApplePayButtonStyle

A type that indicates the available appearances for an Apple Pay Button.

ApplePayButtonLocale

A type that indicates the languages and regions that you can specify for the Apple Pay button.

