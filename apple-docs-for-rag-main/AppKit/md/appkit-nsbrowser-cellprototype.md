

- AppKit
- NSBrowser
-  cellPrototype 

Instance Property

# cellPrototype

The prototype `NSCell` for displaying items in the matrices in the columns of the browser.

macOS

``` source
@MainActor
var cellPrototype: Any! { get set }
```

## Discussion

The prototype `NSCell` instance is copied to display items in the matrices of the browser.

## See Also

### Managing Component Types

class var cellClass: AnyClass

Returns the `NSBrowserCell` class.

func setCellClass(AnyClass)

Sets the class of the cell to be used by the matrices in the columns of the browser.

