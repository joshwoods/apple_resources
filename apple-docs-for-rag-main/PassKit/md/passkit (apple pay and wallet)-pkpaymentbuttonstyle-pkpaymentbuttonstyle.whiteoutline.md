

- PassKit (Apple Pay and Wallet)
- PKPaymentButtonStyle
-  PKPaymentButtonStyle.whiteOutline 

Case

# PKPaymentButtonStyle.whiteOutline

A white button with black lettering and a black outline.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
case whiteOutline
```

## Discussion

Use the white button with black outline on white or very light backgrounds that don’t provide sufficient contrast for a plain white button. Don’t place this button on dark or saturated color backgrounds. Use the white button instead.

In many cases, you can choose either the white button with black outline or the black button. Select the button that works best with your user interface. Always use a single style throughout your app.

## See Also

### Payment button styles

case white

A white button with black lettering.

case black

A black button with white lettering.

case automatic

A button that automatically changes its appearance when the user switches between Light Mode and Dark Mode.

