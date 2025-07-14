

- Speech
- SFSpeechRecognizer
-  locale 

Instance Property

# locale

The locale of the speech recognizer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var locale: Locale { get }
```

## Discussion

The locale of the speech recognizer is an NSLocale object. The default value of this property is the system locale (that is, system).

## See Also

### Getting the Current Language

class func supportedLocales() -> Set&lt;Locale>

Returns the set of locales that are supported by the speech recognizer.

