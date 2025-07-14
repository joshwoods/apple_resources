

- PassKit (Apple Pay and Wallet)
- PKPaymentButton
-  init(paymentButtonType:paymentButtonStyle:) 

Initializer

# init(paymentButtonType:paymentButtonStyle:)

Creates a new payment button with the specified type and style.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
@MainActor
init(
    paymentButtonType type: PKPaymentButtonType,
    paymentButtonStyle style: PKPaymentButtonStyle
)
```

## Parameters 

`type`  

The button’s content. For a complete list of button types, see PKPaymentButtonType.

`style`  

The button’s appearance. For a complete list of button styles, see PKPaymentButtonStyle.

## Return Value

Returns a `PKPaymentButton` instance with the specified type and style.

