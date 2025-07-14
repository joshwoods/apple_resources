

- UIKit
- UITextSearching
-  replaceAll(queryString:options:withText:) 

Instance Method

# replaceAll(queryString:options:withText:)

Informs the searchable object to replace all matching text across all searchable documents.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func replaceAll(
    queryString: String,
    options: UITextSearchOptions,
    withText: String
)
```

**Required** Default implementation provided.

## Parameters 

`queryString`  

The string to search for and replace.

`options`  

The configurable options to use for matching words and comparing strings.

`withText`  

The string to replace the text with.

## Discussion

When supportsTextReplacement returns `YES,` the system calls this method during a find session to request the replacement of all text matching the query string.

## Default Implementations

### UITextSearching Implementations

func replaceAll(queryString: String, options: UITextSearchOptions, withText: String)

## See Also

### Handling replacements

var supportsTextReplacement: Bool

A Boolean value that indicates whether the searchable object supports replacing text.

**Required** Default implementation provided.

func replace(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, withText: String)

Informs the searchable object to replace the text range for the highlighted search result.

**Required** Default implementation provided.

func shouldReplace(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, withText: String) -> Bool

Determines whether the searchable object allows replacement of the text range you provide.

**Required** Default implementation provided.

