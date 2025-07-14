

- UIKit
- UITextSearching
-  replace(foundTextRange:document:withText:) 

Instance Method

# replace(foundTextRange:document:withText:)

Informs the searchable object to replace the text range for the highlighted search result.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func replace(
    foundTextRange: UITextRange,
    document: Self.DocumentIdentifier?,
    withText: String
)
```

**Required** Default implementation provided.

## Parameters 

`foundTextRange`  

The text range to replace.

`document`  

A string that uniquely identifies a document when searching multiple documents, or `nil` when searching a single document.

`withText`  

The string to replace the text with.

## Discussion

When supportsTextReplacement returns `YES,` the system calls this method during a find session to request a text range to replace.

## Default Implementations

### UITextSearching Implementations

func replace(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, withText: String)

## See Also

### Handling replacements

var supportsTextReplacement: Bool

A Boolean value that indicates whether the searchable object supports replacing text.

**Required** Default implementation provided.

func replaceAll(queryString: String, options: UITextSearchOptions, withText: String)

Informs the searchable object to replace all matching text across all searchable documents.

**Required** Default implementation provided.

func shouldReplace(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, withText: String) -> Bool

Determines whether the searchable object allows replacement of the text range you provide.

**Required** Default implementation provided.

