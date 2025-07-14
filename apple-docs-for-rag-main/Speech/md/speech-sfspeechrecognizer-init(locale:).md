

- Speech
- SFSpeechRecognizer
-  init(locale:) 

Initializer

# init(locale:)

Creates a speech recognizer associated with the specified locale.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
init?(locale: Locale)
```

## Parameters 

`locale`  

The locale object representing the language you want to use for speech recognition. For a list of languages supported by the speech recognizer, see supportedLocales().

## Return Value

An initialized speech recognizer object, or `nil` if the specified language was not supported.

## Discussion

If you specify a language that is not supported by the speech recognizer, this method attempts to fall back to the language used by the keyboard for dictation. If that fails, this method returns `nil`.

Even if this method returns a valid speech recognizer object, the speech recognition services may be temporarily unavailable. To determine whether speech recognition services are available, check the isAvailable property.

## See Also

### Creating a Speech Recognizer

convenience init?()

Creates a speech recognizer associated with the user’s default language settings.

