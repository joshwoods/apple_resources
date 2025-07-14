

- BrowserEngineKit
- BETextInteraction
-  transliterateChinese(forText:) 

Instance Method

# transliterateChinese(forText:)

Converts the text between traditional and simplified Chinese.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func transliterateChinese(forText text: String)
```

## Parameters 

`text`  

The text to transliterate.

## Overview

Call this method to get the operating system’s standard transliteration, for example, when your browser text view receives transliterateChinese(_:).

## See Also

### Translation and transliteration

func translate(text: String, from: CGRect)

Presents a translation of the text.

