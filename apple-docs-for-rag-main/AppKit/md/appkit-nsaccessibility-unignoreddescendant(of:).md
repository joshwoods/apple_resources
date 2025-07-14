

- AppKit
- NSAccessibility
-  unignoredDescendant(of:) 

Type Method

# unignoredDescendant(of:)

Returns an unignored accessibility object, descending the hierarchy, if necessary.

macOS

``` source
static func unignoredDescendant(of element: Any) -> Any?
```

## Discussion

Tests whether `element` is an ignored object, returning either `element`, if it is not ignored, or the first unignored descendant of `element`. Use this function only if you know there is a linear, one-to-one, hierarchy below `element`. Otherwise, if `element` has either no unignored children or multiple unignored children, this function fails and returns `nil`.

## See Also

### Getting Accessibility Objects

static func unignoredAncestor(of: Any) -> Any?

Returns an unignored accessibility object, ascending the hierarchy, if necessary.

static func unignoredChildren(from: [Any]) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

static func unignoredChildrenForOnlyChild(from: Any) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

