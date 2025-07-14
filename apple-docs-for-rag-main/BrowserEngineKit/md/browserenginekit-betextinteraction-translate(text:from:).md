

- BrowserEngineKit
- BETextInteraction
-  translate(text:from:) 

Instance Method

# translate(text:from:)

Presents a translation of the text.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func translate(
    text: String,
    from presentationRect: CGRect
)
```

## Parameters 

`text`  

The text to translate.

`presentationRect`  

The area in the text input view in which the text appears, which the operating system uses to locate the translation UI.

## See Also

### Translation and transliteration

func transliterateChinese(forText: String)

Converts the text between traditional and simplified Chinese.

