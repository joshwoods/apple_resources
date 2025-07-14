

- AppKit
- NSSpeechRecognizer
-  blocksOtherRecognizers 

Instance Property

# blocksOtherRecognizers

A Boolean value that indicates whether the speech recognizer object should block all other recognizers (that is, other applications attempting to understand spoken commands) when listening.

macOS

``` source
var blocksOtherRecognizers: Bool { get set }
```

## Discussion

When the value of this property is true, all other speech recognition commands on the system are disabled until the speech recognizer is released, listening is stopped, or the property is set to false. Setting this property to true effectively takes over the computer at the expense of other applications using speech recognition, so you should use it only in circumstances that warrant it, such as when listening for a response important to overall system operation or when an application is running in full-screen mode (such as games and presentation software). The default is value of this property is false.

## See Also

### Configuring Speech Recognizers

var commands: [String]?

An array of strings defining the commands for which the speech recognizer object should listen.

var displayedCommandsTitle: String?

The title of the commands section in the Speech Commands window or `nil` if there is no title.

var listensInForegroundOnly: Bool

A Boolean value that indicates whether the speech recognizer object should only enable its commands when its application is the frontmost one.

