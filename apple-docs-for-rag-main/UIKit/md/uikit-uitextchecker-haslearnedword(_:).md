

- UIKit
- UITextChecker
-  hasLearnedWord(\_:) 

Type Method

# hasLearnedWord(\_:)

Returns whether the text checker has learned the specified word.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class func hasLearnedWord(_ word: String) -> Bool
```

## Parameters 

`word`  

A string representing a word.

## Return Value

true if the class has learned the word, otherwise false.

## See Also

### Learning and Ignoring Words

func ignoreWord(String)

Tells the text checker to ignore the specified word when spell-checking.

var ignoredWords: [String]?

Returns the words that the text checker ignores when spell-checking.

class func learnWord(String)

Tells the text checker to learn the specified word so that it doesn’t evaluate it as misspelled.

class func unlearnWord(String)

Tells the text checker to unlearn the specified word.

