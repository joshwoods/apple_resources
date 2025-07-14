

- UIKit
- UITextSearching
-  shouldReplace(foundTextRange:document:withText:) 

Instance Method

# shouldReplace(foundTextRange:document:withText:)

Determines whether the searchable object allows replacement of the text range you provide.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func shouldReplace(
    foundTextRange: UITextRange,
    document: Self.DocumentIdentifier?,
    withText: String
) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`foundTextRange`  

The range of characters in a text container to consider a replacement for.

`document`  

A string that uniquely identifies the document containing the text range.

`withText`  

The string to replace the text with.

## Return Value

Return `No` to prevent the replacement of a particular text range.

## Discussion

Returning `NO` from this method disables the “replace” button in the find panel. If you don’t implement this method, the system assumes all results are replacable.

## Default Implementations

### UITextSearching Implementations

func shouldReplace(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, withText: String) -> Bool

## See Also

### Handling replacements

var supportsTextReplacement: Bool

A Boolean value that indicates whether the searchable object supports replacing text.

**Required** Default implementation provided.

func replace(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, withText: String)

Informs the searchable object to replace the text range for the highlighted search result.

**Required** Default implementation provided.

func replaceAll(queryString: String, options: UITextSearchOptions, withText: String)

Informs the searchable object to replace all matching text across all searchable documents.

**Required** Default implementation provided.

