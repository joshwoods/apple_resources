

- UIKit
- UITextSearching
-  supportsTextReplacement 

Instance Property

# supportsTextReplacement

A Boolean value that indicates whether the searchable object supports replacing text.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
var supportsTextReplacement: Bool { get }
```

**Required** Default implementation provided.

## Default Implementations

### UITextSearching Implementations

var supportsTextReplacement: Bool

## See Also

### Handling replacements

func replace(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, withText: String)

Informs the searchable object to replace the text range for the highlighted search result.

**Required** Default implementation provided.

func replaceAll(queryString: String, options: UITextSearchOptions, withText: String)

Informs the searchable object to replace all matching text across all searchable documents.

**Required** Default implementation provided.

func shouldReplace(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, withText: String) -> Bool

Determines whether the searchable object allows replacement of the text range you provide.

**Required** Default implementation provided.

