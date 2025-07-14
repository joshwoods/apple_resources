

- AppKit
-  NSSpeechRecognizer 

Class

# NSSpeechRecognizer

The Cocoa interface to speech recognition in macOS.

macOS

``` source
class NSSpeechRecognizer
```

## Overview

NSSpeechRecognizer provides a “command and control” style of voice recognition system, where the command phrases must be defined prior to listening, in contrast to a dictation system where the recognized text is unconstrained. Through an NSSpeechRecognizer instance, Cocoa apps can use the speech recognition engine built into macOS to recognize spoken commands. With speech recognition, users can accomplish complex tasks with spoken commands—for example, “Move pawn B2 to B4” and “Take back move.”

The NSSpeechRecognizer class has a property that lets you specify which spoken words should be recognized as commands (commands) and methods that let you start and stop listening (startListening() and stopListening()). When the speech recognition facility recognizes one of the designated commands, NSSpeechRecognizer invokes the delegation method speechRecognizer(_:didRecognizeCommand:), allowing the delegate to perform the command.

Speech recognition is just one of the macOS speech technologies. The speech synthesis technology allows applications to “pronounce” written text in U.S. English and over 25 other languages, with a number of different voices and dialects for each language (NSSpeechSynthesizer is the Cocoa interface to this technology). Both speech technologies provide benefits for all users, and are particularly useful to those users who have difficulties seeing the screen or using the mouse and keyboard. By incorporating speech into your application, you can provide a concurrent mode of interaction for your users: In macOS, your software can accept input and provide output without requiring users to change their working context.

## Topics

### Creating Speech Recognizers

init?()

Initializes and returns an instance of the `NSSpeechRecognizer` class.

### Handling the Recognition of a Spoken Command

var delegate: (any NSSpeechRecognizerDelegate)?

The delegate for the speech recognizer object.

protocol NSSpeechRecognizerDelegate

A set of optional methods implemented by delegates of NSSpeechRecognizer objects.

### Configuring Speech Recognizers

var commands: [String]?

An array of strings defining the commands for which the speech recognizer object should listen.

var displayedCommandsTitle: String?

The title of the commands section in the Speech Commands window or `nil` if there is no title.

var listensInForegroundOnly: Bool

A Boolean value that indicates whether the speech recognizer object should only enable its commands when its application is the frontmost one.

var blocksOtherRecognizers: Bool

A Boolean value that indicates whether the speech recognizer object should block all other recognizers (that is, other applications attempting to understand spoken commands) when listening.

### Listening

func startListening()

Tells the speech recognition engine to begin listening for commands.

func stopListening()

Tells the speech recognition engine to suspend listening for commands.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Speech

class NSSpeechSynthesizer

The Cocoa interface to speech synthesis in macOS.

Deprecated

