

- PassKit (Apple Pay and Wallet)
- PKPaymentButton
-  cornerRadius 

Instance Property

# cornerRadius

The radius, in points, for the rounded corners on the button.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
@MainActor
var cornerRadius: CGFloat { get set }
```

## Discussion

To remove the rounded corners, set this value to 0.0.

The default value is `4.0`.

## See Also

### Configuring the appearance

enum PKPaymentButtonType

The Apple Pay button types you can display to initiate Apple Pay transactions.

enum PKPaymentButtonStyle

A type that indicates the available appearances for an Apple Pay button.

