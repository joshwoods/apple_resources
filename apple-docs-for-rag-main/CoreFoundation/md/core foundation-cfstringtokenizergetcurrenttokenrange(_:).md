

- Core Foundation
-  CFStringTokenizerGetCurrentTokenRange(\_:) 

Function

# CFStringTokenizerGetCurrentTokenRange(\_:)

Returns the range of the current token.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFStringTokenizerGetCurrentTokenRange(_ tokenizer: CFStringTokenizer!) -> CFRange
```

## Parameters 

`tokenizer`  

A CFStringTokenizer object.

## Return Value

The range of the current token, or ``` {``kCFNotFound ```, `0}` if there is no current token.

## See Also

### Getting Information About the Current Token

func CFStringTokenizerCopyCurrentTokenAttribute(CFStringTokenizer!, CFOptionFlags) -> CFTypeRef!

Returns a given attribute of the current token.

func CFStringTokenizerGetCurrentSubTokens(CFStringTokenizer!, UnsafeMutablePointer&lt;CFRange>!, CFIndex, CFMutableArray!) -> CFIndex

Retrieves the subtokens or derived subtokens contained in the compound token.

