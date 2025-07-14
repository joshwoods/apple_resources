

- Core Foundation
-  CFStringTokenizerCopyCurrentTokenAttribute(\_:\_:) 

Function

# CFStringTokenizerCopyCurrentTokenAttribute(\_:\_:)

Returns a given attribute of the current token.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFStringTokenizerCopyCurrentTokenAttribute(
    _ tokenizer: CFStringTokenizer!,
    _ attribute: CFOptionFlags
) -> CFTypeRef!
```

## Parameters 

`tokenizer`  

A CFStringTokenizer object.

`attribute`  

The token attribute to obtain. The value must be `kCFStringTokenizerAttributeLatinTranscription`, or `kCFStringTokenizerAttributeLanguage`.

## Return Value

The attribute specified by `attribute` of the current token, or `NULL` if the current token does not have the specified attribute or there is no current token. Ownership follows the The Create Rule.

## See Also

### Getting Information About the Current Token

func CFStringTokenizerGetCurrentTokenRange(CFStringTokenizer!) -> CFRange

Returns the range of the current token.

func CFStringTokenizerGetCurrentSubTokens(CFStringTokenizer!, UnsafeMutablePointer&lt;CFRange>!, CFIndex, CFMutableArray!) -> CFIndex

Retrieves the subtokens or derived subtokens contained in the compound token.

