

- Media Player
- MPFeedbackCommand
-  isActive 

Instance Property

# isActive

A Boolean value that indicates whether the feedback’s action is on or off.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
var isActive: Bool { get set }
```

## Discussion

When set to true, feedback is available. Use this property to get or set the current state of the given feedback. An example of an active feedback command is a Like button that has been enabled by the user. In that scenario, toggling the button on and off would similarly toggle the value in this property.

## See Also

### Retrieving information about a feedback command

var localizedTitle: String

A localized string used to describe the context of a command.

var localizedShortTitle: String

A shortened version of the string used to describe the context of a command.

