

- WatchKit
-  WKAlertActionStyle 

Enumeration

# WKAlertActionStyle

Constants indicating the style of the action button.

watchOS 2.0+

``` source
enum WKAlertActionStyle
```

## Topics

### Constants

case `default`

The default style. Use this for most of your buttons.

case cancel

A cancel action. Use this style for an action that cancels the operation without making changes.

case destructive

An action that causes destructive behavior to the user’s data or the app. Destructive actions are styled in a way that warns the user of the destructive nature of the action.

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

### Constants

typealias WKAlertActionHandler

A block to perform in response to an action.

