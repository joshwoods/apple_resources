

- WebKit
- WebView
-  search(for:direction:caseSensitive:wrap:) Deprecated

Instance Method

# search(for:direction:caseSensitive:wrap:)

Searches a document view for a string and highlights it if it is found.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func search(
    for string: String!,
    direction forward: Bool,
    caseSensitive caseFlag: Bool,
    wrap wrapFlag: Bool
) -> Bool
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`string`  

The search string.

`forward`  

If true the direction of the search is forward; if false, the direction is backward.

`caseFlag`  

If true if the search is case sensitive; otherwise, it is not.

`wrapFlag`  

If true if the search wraps; otherwise, it does not.

## Return Value

true if the search is successful; otherwise, false.

## Discussion

The search for `string` begins from the current selection and continues in the direction specified by `forward`. The search continues across all frames.

## See Also

### Related Documentation

var applicationNameForUserAgent: String!

The receiver’s application name that is used in the user-agent string.

Deprecated

var customUserAgent: String!

The receiver’s custom user-agent string.

Deprecated

