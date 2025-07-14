

- UIKit
- UITextChecker
-  unlearnWord(\_:) 

Type Method

# unlearnWord(\_:)

Tells the text checker to unlearn the specified word.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class func unlearnWord(_ word: String)
```

## Parameters 

`word`  

A string representing the word for the class to unlearn.

## Discussion

When a `UITextChecker` object unlearns a word, it is removed from the dictionary.

## See Also

### Learning and Ignoring Words

func ignoreWord(String)

Tells the text checker to ignore the specified word when spell-checking.

var ignoredWords: [String]?

Returns the words that the text checker ignores when spell-checking.

class func learnWord(String)

Tells the text checker to learn the specified word so that it doesn’t evaluate it as misspelled.

class func hasLearnedWord(String) -> Bool

Returns whether the text checker has learned the specified word.

