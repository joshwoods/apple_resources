

- AppKit
- NSAccessibility
-  unignoredChildren(from:) 

Type Method

# unignoredChildren(from:)

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

macOS

``` source
static func unignoredChildren(from originalChildren: [Any]) -> [Any]
```

## Discussion

This function first tests whether `originalChildren` contains any ignored objects. If the array contains no ignored objects, the function returns `originalChildren`. If the array contains ignored objects, this function returns a new array that contains the contents of `originalChildren`, but with each ignored object replaced by its unignored descendant.

## See Also

### Getting Accessibility Objects

static func unignoredAncestor(of: Any) -> Any?

Returns an unignored accessibility object, ascending the hierarchy, if necessary.

static func unignoredChildrenForOnlyChild(from: Any) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

static func unignoredDescendant(of: Any) -> Any?

Returns an unignored accessibility object, descending the hierarchy, if necessary.

