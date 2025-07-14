

- AppKit
- NSSpeechRecognizer
-  listensInForegroundOnly 

Instance Property

# listensInForegroundOnly

A Boolean value that indicates whether the speech recognizer object should only enable its commands when its application is the frontmost one.

macOS

``` source
var listensInForegroundOnly: Bool { get set }
```

## Discussion

When the value of this property is true, the speech recognizer’s commands are only recognized when the speech recognizer’s application is the frontmost application—typically the application displaying the menu bar. If the value of the property is false, the commands are recognized regardless of the visibility of the application, including agent applications (agent applications, which have the `LSUIElement` property set, do not appear in the Dock or Force Quit window). The default value of this property is true.

## See Also

### Configuring Speech Recognizers

var commands: [String]?

An array of strings defining the commands for which the speech recognizer object should listen.

var displayedCommandsTitle: String?

The title of the commands section in the Speech Commands window or `nil` if there is no title.

var blocksOtherRecognizers: Bool

A Boolean value that indicates whether the speech recognizer object should block all other recognizers (that is, other applications attempting to understand spoken commands) when listening.

