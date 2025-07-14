

- ManagedAppDistribution
- ManagedApp
-  languages 

Instance Property

# languages

The app’s supported languages.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
let languages: [Locale.Language]
```

## Discussion

Tip

Use `Locale.localizedString(forLanguageCode:)` to obtain a display name for the language, using metadataLanguage to create the `Locale`.

## See Also

### Obtaining supported languages

let metadataLanguage: Locale.Language?

The language of the localized properties of this managed app.

