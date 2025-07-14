

- PassKit (Apple Pay and Wallet)
-  PKPayLaterDisplayStyle Deprecated

Enumeration

# PKPayLaterDisplayStyle

Values you use to style an Apple Pay Later visual merchandising widget.

iOS 17.0+iPadOS 17.0+visionOS 1.0+

``` source
enum PKPayLaterDisplayStyle
```

Deprecated

Apple Pay Later is deprecated.

## Topics

### Payment view display styles

case standard

The standard Apple Pay Later visual merchandising widget style.

case badge

Displays a badge that uses an Apple Pay Later icon.

case checkout

A style used inside of a checkout view that presents Apple Pay and other payment options to the customer.

case price

A style that shows the Apple Pay Later view beneath a product’s price.

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

### Styling the view

var displayStyle: PKPayLaterDisplayStyle

The style to use when presenting the Apple Pay Later visual merchandising widget view.

Deprecated

