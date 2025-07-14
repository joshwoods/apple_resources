

- Core Foundation
-  CFStringTokenizerAdvanceToNextToken(\_:) 

Function

# CFStringTokenizerAdvanceToNextToken(\_:)

Advances the tokenizer to the next token and sets that as the current token.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFStringTokenizerAdvanceToNextToken(_ tokenizer: CFStringTokenizer!) -> CFStringTokenizerTokenType
```

## Parameters 

`tokenizer`  

A CFStringTokenizer object.

## Return Value

The type of the token if the tokenizer succeeded in finding a token and setting it as current token. Returns `kCFStringTokenizerTokenNone` if the tokenizer failed to find a token. For possible values, see CFStringTokenizerTokenType.

## Discussion

If there is no preceding call to CFStringTokenizerGoToTokenAtIndex(_:_:) or CFStringTokenizerAdvanceToNextToken(_:), the function finds the first token in the range specified by the CFStringTokenizerCreate(_:_:_:_:_:). If there is a preceding, successful, call to CFStringTokenizerGoToTokenAtIndex(_:_:) or CFStringTokenizerAdvanceToNextToken(_:) and there is a current token, proceeds to the next token. If a token is found, it is set as the current token and the function returns `true`; otherwise the current token is invalidated and the function returns `false`.

You can obtain the range and attribute of the token calling CFStringTokenizerGetCurrentTokenRange(_:) and CFStringTokenizerCopyCurrentTokenAttribute(_:_:). If the token is a compound (with type `kCFStringTokenizerTokenHasSubTokensMask` or `kCFStringTokenizerTokenHasDerivedSubTokensMask`), you can obtain its subtokens and (or) derived subtokens by calling CFStringTokenizerGetCurrentSubTokens(_:_:_:_:).

## See Also

### Changing the Location

func CFStringTokenizerGoToTokenAtIndex(CFStringTokenizer!, CFIndex) -> CFStringTokenizerTokenType

Finds a token that includes the character at a given index, and set it as the current token.

