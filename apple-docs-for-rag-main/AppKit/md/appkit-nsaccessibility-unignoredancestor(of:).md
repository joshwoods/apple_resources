

- AppKit
- NSAccessibility
-  unignoredAncestor(of:) 

Type Method

# unignoredAncestor(of:)

Returns an unignored accessibility object, ascending the hierarchy, if necessary.

macOS

``` source
static func unignoredAncestor(of element: Any) -> Any?
```

## Discussion

Tests whether `element` is an ignored object, returning either `element`, if it is not ignored, or the first unignored ancestor of `element`.

## See Also

### Getting Accessibility Objects

static func unignoredChildren(from: [Any]) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

static func unignoredChildrenForOnlyChild(from: Any) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

static func unignoredDescendant(of: Any) -> Any?

Returns an unignored accessibility object, descending the hierarchy, if necessary.

