

- Media Player
- MPFeedbackCommand
-  localizedTitle 

Instance Property

# localizedTitle

A localized string used to describe the context of a command.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
var localizedTitle: String { get set }
```

## Discussion

Use this property to store the text you want shown to the user in conjunction with this command. For example, you might assign the string “I like this” to this property for the command associated with a Like button. The text you specify is displayed to the user at appropriate times by the system.

## See Also

### Retrieving information about a feedback command

var isActive: Bool

A Boolean value that indicates whether the feedback’s action is on or off.

var localizedShortTitle: String

A shortened version of the string used to describe the context of a command.

