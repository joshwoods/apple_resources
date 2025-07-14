

- AppKit
- NSAccessibility
-  unignoredChildrenForOnlyChild(from:) 

Type Method

# unignoredChildrenForOnlyChild(from:)

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

macOS

``` source
static func unignoredChildrenForOnlyChild(from originalChild: Any) -> [Any]
```

## Discussion

Tests whether `originalChild` is an ignored object and returns an array containing either `originalChild`, if it is not ignored, or its unignored descendants.

## See Also

### Getting Accessibility Objects

static func unignoredAncestor(of: Any) -> Any?

Returns an unignored accessibility object, ascending the hierarchy, if necessary.

static func unignoredChildren(from: [Any]) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

static func unignoredDescendant(of: Any) -> Any?

Returns an unignored accessibility object, descending the hierarchy, if necessary.

