

- AppKit
- NSBrowserCell
-  branchImage 

Type Property

# branchImage

Returns the default image for branch cells in a browser.

macOS

``` source
@MainActor
class var branchImage: NSImage? { get }
```

## Return Value

The default image used for branch `NSBrowserCell` objects. The default image is a right-pointing triangle.

## Discussion

Override this method if you want a different image. To have a branch `NSBrowserCell` with no image (and no space reserved for an image), override this method to return `nil`.

## See Also

### Related Documentation

Browser Programming Topics

var alternateImage: NSImage?

The browser cell’s image for the highlighted state.

### Getting Browser Cell Information

class var highlightedBranchImage: NSImage?

Returns the default image for branch browser cells that are highlighted.

