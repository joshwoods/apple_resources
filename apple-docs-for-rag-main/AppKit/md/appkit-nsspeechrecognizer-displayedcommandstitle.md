

- AppKit
- NSSpeechRecognizer
-  displayedCommandsTitle 

Instance Property

# displayedCommandsTitle

The title of the commands section in the Speech Commands window or `nil` if there is no title.

macOS

``` source
var displayedCommandsTitle: String? { get set }
```

## Discussion

When this property is a non-empty string, commands are displayed in the Speech Commands window indented under a section with this title. If `title` is `nil` or an empty string, the commands are displayed at the top level of the Speech Commands window. This default is not to display the commands under a section title.

## See Also

### Configuring Speech Recognizers

var commands: [String]?

An array of strings defining the commands for which the speech recognizer object should listen.

var listensInForegroundOnly: Bool

A Boolean value that indicates whether the speech recognizer object should only enable its commands when its application is the frontmost one.

var blocksOtherRecognizers: Bool

A Boolean value that indicates whether the speech recognizer object should block all other recognizers (that is, other applications attempting to understand spoken commands) when listening.

