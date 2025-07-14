

- UIKit
- UIContextualAction
-  UIContextualAction.Style 

Enumeration

# UIContextualAction.Style

Constants indicating the style information that applies to the action button.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Style
```

## Topics

### Styles

case normal

A normal action.

case destructive

An action that deletes data or performs some type of destructive task.

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

### Getting the configuration details

var handler: UIContextualAction.Handler

The handler block to execute when the user selects the action.

typealias Handler

The handler block to call in response to the selection of an action.

var style: UIContextualAction.Style

The style that applies to the action button.

