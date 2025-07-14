

- Speech
- SFSpeechRecognizer
-  init() 

Initializer

# init()

Creates a speech recognizer associated with the user’s default language settings.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
convenience init?()
```

## Return Value

An initialized speech recognizer object, or `nil` if there was a problem creating the object.

## Discussion

If the user’s default language is not supported for speech recognition, this method attempts to fall back to the language used by the keyboard for dictation. If that fails, this method returns `nil`.

Even if this method returns a valid speech recognizer object, the speech recognition services may be temporarily unavailable. To determine whether speech recognition services are available, check the isAvailable property.

## See Also

### Creating a Speech Recognizer

init?(locale: Locale)

Creates a speech recognizer associated with the specified locale.

