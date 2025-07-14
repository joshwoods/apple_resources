

- AppKit
- NSBrowser
-  setCellClass(\_:) 

Instance Method

# setCellClass(\_:)

Sets the class of the cell to be used by the matrices in the columns of the browser.

macOS

``` source
@MainActor
func setCellClass(_ factoryId: AnyClass)
```

## Parameters 

`factoryId`  

The class of `NSCell` used by the matrices in the columns of the browser. This method creates an instance of the class and sets cellPrototype.

## See Also

### Managing Component Types

class var cellClass: AnyClass

Returns the `NSBrowserCell` class.

var cellPrototype: Any!

The prototype `NSCell` for displaying items in the matrices in the columns of the browser.

