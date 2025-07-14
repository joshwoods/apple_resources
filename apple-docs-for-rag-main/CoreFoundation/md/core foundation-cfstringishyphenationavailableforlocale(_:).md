

- Core Foundation
-  CFStringIsHyphenationAvailableForLocale(\_:) 

Function

# CFStringIsHyphenationAvailableForLocale(\_:)

Returns a Boolean value that indicates whether hyphenation data is available.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFStringIsHyphenationAvailableForLocale(_ locale: CFLocale!) -> Bool
```

## Parameters 

`locale`  

A valid locale that specifies which language’s hyphenation conventions to use. Hyphenation data is not available for all locales.

## See Also

### Working With Hyphenation

func CFStringGetHyphenationLocationBeforeIndex(CFString!, CFIndex, CFRange, CFOptionFlags, CFLocale!, UnsafeMutablePointer&lt;UTF32Char>!) -> CFIndex

Retrieve the first potential hyphenation location found before the specified location.

