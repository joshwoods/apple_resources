

- Core Foundation
-  CFLocaleGetLanguageCharacterDirection(\_:) 

Function

# CFLocaleGetLanguageCharacterDirection(\_:)

Returns the character direction for the specified ISO language code.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFLocaleGetLanguageCharacterDirection(_ isoLangCode: CFString!) -> CFLocaleLanguageDirection
```

## Parameters 

`isoLangCode`  

The ISO language code.

## Return Value

The character direction for the language. See CFLocaleLanguageDirection for possible values. If the appropriate direction can’t be determined, CFLocaleLanguageDirection.unknown is returned.

## See Also

### Getting Line and Character Direction for a Language

func CFLocaleGetLanguageLineDirection(CFString!) -> CFLocaleLanguageDirection

Returns the line direction for the specified ISO language code.

