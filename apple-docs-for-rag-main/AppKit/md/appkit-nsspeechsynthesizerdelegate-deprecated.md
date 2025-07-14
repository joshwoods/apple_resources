

- AppKit
-  NSSpeechSynthesizerDelegate Deprecated

Protocol

# NSSpeechSynthesizerDelegate

A set of optional methods implemented by delegates of NSSpeechSynthesizer objects.

macOS 10.3–14.0Deprecated

``` source
protocol NSSpeechSynthesizerDelegate : NSObjectProtocol
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Topics

### Synthesizing Speech

func speechSynthesizer(NSSpeechSynthesizer, willSpeakWord: NSRange, of: String)

Sent just before a synthesized word is spoken through the sound output device.

func speechSynthesizer(NSSpeechSynthesizer, willSpeakPhoneme: Int16)

Sent just before a synthesized phoneme is spoken through the sound output device.

func speechSynthesizer(NSSpeechSynthesizer, didEncounterErrorAt: Int, of: String, message: String)

Sent to the delegate when a speech synthesizer encounters an error in text being synthesized.

func speechSynthesizer(NSSpeechSynthesizer, didEncounterSyncMessage: String)

Sent to the delegate when a speech synthesizer encounters a synchronization error.

func speechSynthesizer(NSSpeechSynthesizer, didFinishSpeaking: Bool)

Sent when an NSSpeechSynthesizer object finishes speaking through the sound output device.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Customizing the Speech Synthesizer Behavior

var delegate: (any NSSpeechSynthesizerDelegate)?

The synthesizer’s delegate.

Deprecated

