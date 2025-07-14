

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.SpeechPropertyKey
- NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey
-  newestCode 

Type Property

# newestCode

The error code of the most recent error that occurred since the last call to object(forProperty:) with the errors property. An `NSNumber`

macOS 10.5+

``` source
static let newestCode: NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey
```

## See Also

### Type Properties

static let count: NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey

The number of errors that have occurred in processing the current text string, since the last call to object(forProperty:) with the errors property. An `NSNumber`

static let newestCharacterOffset: NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey

The position in the text string of the most recent error that occurred since the last call to object(forProperty:) with the errors property. An `NSNumber`.

static let oldestCharacterOffset: NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey

The position in the text string of the first error that occurred since the last call to object(forProperty:) with the errors property. An `NSNumber`

static let oldestCode: NSSpeechSynthesizer.SpeechPropertyKey.ErrorKey

The error code of the first error that occurred since the last call to object(forProperty:) with the errors property. An `NSNumber`

