

- CarPlay
- CPAlertAction
-  CPAlertAction.Style 

Enumeration

# CPAlertAction.Style

Display styles for an alert’s action button.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
enum Style
```

## Topics

### Styles

case `default`

The default display style for an action button.

case cancel

The display style indicating that the action leaves data unchanged.

case destructive

The style indicating that the action changes or deletes data.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Action Style

var style: CPAlertAction.Style

The display style for the action button.

