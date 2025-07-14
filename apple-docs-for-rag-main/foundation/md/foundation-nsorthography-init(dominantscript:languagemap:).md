

- Foundation
- NSOrthography
-  init(dominantScript:languageMap:) 

Initializer

# init(dominantScript:languageMap:)

Creates an orthography object with the specified dominant script and language map.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    dominantScript script: String,
    languageMap map: [String : [String]]
)
```

## Parameters 

`script`  

The dominant script.

`map`  

A dictionary mapping ISO 15924 script codes to arrays of BCP-47 language tags.

## Return Value

An orthography object initialized with the specified script and language map.

## Discussion

You typically use the defaultOrthography(forLanguage:) method to create orthography objects with automatic language mapping. Use this initializer only if you need to override the script associated with one or more languages.

## See Also

### Creating Orthography Objects

class func defaultOrthography(forLanguage: String) -> Self

Creates and returns an orthography object with the default language map for the specified language.

