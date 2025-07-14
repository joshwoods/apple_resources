

- AppKit
- NSBrowserCell
-  highlightedBranchImage 

Type Property

# highlightedBranchImage

Returns the default image for branch browser cells that are highlighted.

macOS

``` source
@MainActor
class var highlightedBranchImage: NSImage? { get }
```

## Return Value

The default image used for branch `NSBrowserCell` objects that are highlighted. This is a lighter version of the image returned by branchImage.

## Discussion

Override this method if you want a different image.

## See Also

### Related Documentation

var alternateImage: NSImage?

The browser cell’s image for the highlighted state.

### Getting Browser Cell Information

class var branchImage: NSImage?

Returns the default image for branch cells in a browser.

