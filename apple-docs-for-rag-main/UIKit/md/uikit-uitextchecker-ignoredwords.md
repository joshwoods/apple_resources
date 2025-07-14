

- UIKit
- UITextChecker
-  ignoredWords 

Instance Property

# ignoredWords

Returns the words that the text checker ignores when spell-checking.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var ignoredWords: [String]? { get set }
```

## Return Value

An array of strings, each of which specifies a word the receiver ignores when it is spell-checking a document.

## Discussion

The spell checker excludes ignored words as misspelled words during the current spell-checking session only.

## See Also

### Learning and Ignoring Words

func ignoreWord(String)

Tells the text checker to ignore the specified word when spell-checking.

class func learnWord(String)

Tells the text checker to learn the specified word so that it doesn’t evaluate it as misspelled.

class func unlearnWord(String)

Tells the text checker to unlearn the specified word.

class func hasLearnedWord(String) -> Bool

Returns whether the text checker has learned the specified word.

