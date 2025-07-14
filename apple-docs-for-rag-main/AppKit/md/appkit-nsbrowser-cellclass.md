

- AppKit
- NSBrowser
-  cellClass 

Type Property

# cellClass

Returns the `NSBrowserCell` class.

macOS

``` source
@MainActor
class var cellClass: AnyClass { get }
```

## Return Value

Always returns the `NSBrowserCell` class (even if the developer has sent a setCellClass(_:) message to a particular instance).

## Discussion

This method is used by `NSControl` during initialization and is not meant to be used by applications.

## See Also

### Managing Component Types

func setCellClass(AnyClass)

Sets the class of the cell to be used by the matrices in the columns of the browser.

var cellPrototype: Any!

The prototype `NSCell` for displaying items in the matrices in the columns of the browser.

