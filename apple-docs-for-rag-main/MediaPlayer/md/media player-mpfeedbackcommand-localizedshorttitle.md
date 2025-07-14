

- Media Player
- MPFeedbackCommand
-  localizedShortTitle 

Instance Property

# localizedShortTitle

A shortened version of the string used to describe the context of a command.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 2.0+

``` source
var localizedShortTitle: String { get set }
```

## Discussion

Use this property to provide information about a feedback command that is suitable for display when screen space is more constrained. For example, Apple Watch uses this string instead of the string in the localizedTitle property.

## See Also

### Retrieving information about a feedback command

var isActive: Bool

A Boolean value that indicates whether the feedback’s action is on or off.

var localizedTitle: String

A localized string used to describe the context of a command.

