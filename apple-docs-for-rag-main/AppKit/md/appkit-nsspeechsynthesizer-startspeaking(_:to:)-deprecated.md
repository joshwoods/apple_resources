

- AppKit
- NSSpeechSynthesizer
-  startSpeaking(\_:to:) Deprecated

Instance Method

# startSpeaking(\_:to:)

Begins synthesizing text into a sound (AIFF) file.

macOS 10.3–14.0Deprecated

``` source
func startSpeaking(
    _ string: String,
    to url: URL
) -> Bool
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Parameters 

`string`  

Text to speak. When `nil` or empty, no synthesis is started.

`url`  

Filesystem location of the output sound file.

## Return Value

true when synthesis starts successfully, false otherwise.

## Discussion

When synthesis of `text` finishes normally or is stopped, the message speechSynthesizer(_:didFinishSpeaking:) is sent to the delegate.

One example of how you might use this method is in an email program that automatically converts new messages into sound files that can be stored on an iPod for later listening.

Note

In OS X V 10.4 and earlier, the delegate does not receive speechSynthesizer(_:willSpeakWord:of:) and speechSynthesizer(_:willSpeakPhoneme:) messages when text is being synthesized to a file.

## See Also

### Synthesizing Speech

var isSpeaking: Bool

Indicates whether the receiver is currently generating synthesized speech.

Deprecated

func startSpeaking(String) -> Bool

Begins speaking synthesized text through the system’s default sound output device.

Deprecated

func pauseSpeaking(at: NSSpeechSynthesizer.Boundary)

Pauses synthesis in progress at a given boundary.

Deprecated

func continueSpeaking()

Resumes synthesis.

Deprecated

func stopSpeaking()

Stops synthesis in progress.

Deprecated

func stopSpeaking(at: NSSpeechSynthesizer.Boundary)

Stops synthesis in progress at a given boundary.

Deprecated

enum Boundary

These constants are used to indicate where speech should be stopped and paused. See pauseSpeaking(at:) and stopSpeaking(at:).

Deprecated

