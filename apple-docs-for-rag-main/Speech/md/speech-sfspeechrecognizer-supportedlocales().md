

- Speech
- SFSpeechRecognizer
-  supportedLocales() 

Type Method

# supportedLocales()

Returns the set of locales that are supported by the speech recognizer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class func supportedLocales() -> Set
```

## Return Value

A set of locales that support speech recognition.

## Discussion

This method returns the locales for which speech recognition is supported. Support for a locale does not guarantee that speech recognition is currently possible for that locale. For some locales, the speech recognizer requires an active Internet connection to communicate with Apple’s servers. If the speech recognizer is currently unable to process requests, isAvailable returns false.

Speech recognition supports the same locales that are supported by the keyboard’s dictation feature. For a list of these locales, see QuickType Keyboard: Dictation.

## See Also

### Getting the Current Language

var locale: Locale

The locale of the speech recognizer.

