

- WebKit
- WebDocumentSearching
-  search(for:direction:caseSensitive:wrap:) Deprecated

Instance Method

# search(for:direction:caseSensitive:wrap:)

Searches for a string in a given direction from the current position.

macOS 10.3–10.14Deprecated

``` source
func search(
    for string: String!,
    direction forward: Bool,
    caseSensitive caseFlag: Bool,
    wrap wrapFlag: Bool
) -> Bool
```

**Required**

## Parameters 

`string`  

The string to search for.

`forward`  

If true, the search is in the forward direction from the current location; otherwise, the search is in the backward direction.

`caseFlag`  

If true then the search is case sensitive; otherwise, it is not.

`wrapFlag`  

If true, the search continues from the end of the document to the current location; otherwise, it stops at the end of the document.

## Return Value

true if the receiver contains `string` in the specified direction; otherwise, false.

## Discussion

The receiver should select the string if it is found.

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

