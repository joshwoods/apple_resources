

- MapKit JS
- MapKitInitOptions
-  language 

Instance Property

# language

An ID that indicates the preferred language to use when displaying map labels, controls, directions, and other text.

MapKit JS 5.0+

``` source
attribute string language;
```

## Discussion

The language ID lets you indicate the language to use for displaying map labels, controls, error messages, and search and directions text. A language ID consists of a language designator followed by an optional region or script designator. Some examples of language IDs are:

- `de` (German)

- `es-MX` (Mexican Spanish)

- `zh-Hans` (simplified Chinese)

- `es` (Spanish)

If the language ID is invalid or missing, MapKit JS uses the language that the user’s browser specifies. If MapKit JS doesn’t support the preferred language, the language defaults to English.

For more information about language IDs, see Internationalization and Localization Guide.

## See Also

### Callback and language

authorizationCallback

A callback function that obtains a token.

