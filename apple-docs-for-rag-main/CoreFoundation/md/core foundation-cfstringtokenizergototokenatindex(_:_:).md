

- Core Foundation
-  CFStringTokenizerGoToTokenAtIndex(\_:\_:) 

Function

# CFStringTokenizerGoToTokenAtIndex(\_:\_:)

Finds a token that includes the character at a given index, and set it as the current token.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFStringTokenizerGoToTokenAtIndex(
    _ tokenizer: CFStringTokenizer!,
    _ index: CFIndex
) -> CFStringTokenizerTokenType
```

## Parameters 

`tokenizer`  

A CFStringTokenizer object.

`index`  

The index of a character in the string for `tokenizer`.

## Return Value

The type of the token if the tokenizer succeeded in finding a token and setting it as the current token. Returns `kCFStringTokenizerTokenNone` if the tokenizer failed to find a token. For possible values, see CFStringTokenizerTokenType.

## Discussion

You can obtain the range and attribute of the token calling CFStringTokenizerGetCurrentTokenRange(_:) and CFStringTokenizerCopyCurrentTokenAttribute(_:_:). If the token is a compound (with type `kCFStringTokenizerTokenHasSubTokensMask` or `kCFStringTokenizerTokenHasDerivedSubTokensMask`), you can obtain its subtokens and (or) derived subtokens by calling CFStringTokenizerGetCurrentSubTokens(_:_:_:_:).

## See Also

### Changing the Location

func CFStringTokenizerAdvanceToNextToken(CFStringTokenizer!) -> CFStringTokenizerTokenType

Advances the tokenizer to the next token and sets that as the current token.

