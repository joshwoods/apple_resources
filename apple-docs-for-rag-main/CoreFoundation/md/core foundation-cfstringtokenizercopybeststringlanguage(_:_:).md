

- Core Foundation
-  CFStringTokenizerCopyBestStringLanguage(\_:\_:) 

Function

# CFStringTokenizerCopyBestStringLanguage(\_:\_:)

Guesses a language of a given string and returns the guess as a BCP 47 string.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFStringTokenizerCopyBestStringLanguage(
    _ string: CFString!,
    _ range: CFRange
) -> CFString!
```

## Parameters 

`string`  

The string to test to identify the language.

`range`  

The range of `string` to use for the test. If `NULL`, the first few hundred characters of the string are examined.

## Return Value

A language in BCP 47 form, or `NULL` if the language in `string` could not be identified. Ownership follows the The Create Rule.

## Discussion

The result is not guaranteed to be accurate. Typically, the function requires 200-400 characters to reliably guess the language of a string.

CFStringTokenizer recognizes the following languages:

ar (Arabic), bg (Bulgarian), cs (Czech), da (Danish), de (German), el (Greek), en (English), es (Spanish), fi (Finnish), fr (French), he (Hebrew), hr (Croatian), hu (Hungarian), is (Icelandic), it (Italian), ja (Japanese), ko (Korean), nb (Norwegian Bokmål), nl (Dutch), pl (Polish), pt (Portuguese), ro (Romanian), ru (Russian), sk (Slovak), sv (Swedish), th (Thai), tr (Turkish), uk (Ukrainian), zh-Hans (Simplified Chinese), zh-Hant (Traditional Chinese).

