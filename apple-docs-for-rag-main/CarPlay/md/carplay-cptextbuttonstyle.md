

- CarPlay
-  CPTextButtonStyle 

Enumeration

# CPTextButtonStyle

The styles a button can apply to its title to communicate its action.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum CPTextButtonStyle
```

## Topics

### Button Text Styles

case normal

A style that indicates the button performs an action other than to confirm or cancel.

case confirm

A style that indicates the button confirms an action and changes data.

case cancel

A style that indicates the button cancels an action and doesn’t change data.

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

### Managing the Button Style

var textStyle: CPTextButtonStyle

The text style the button applies to its title.

