

- AppKit
- NSNib
-  init(nibData:bundle:) 

Initializer

# init(nibData:bundle:)

Initializes an instance with nib data and specified bundle for locating resources.

macOS 10.8+

``` source
init(
    nibData: Data,
    bundle: Bundle?
)
```

## Parameters 

`nibData`  

The nib data.

`bundle`  

The bundle for locating resources. If `nil`, the main application bundle is used.

## Return Value

The initialized `NSNib` object or `nil` if there were errors during initialization.

## See Also

### Initializing a Nib

init?(nibNamed: NSNib.Name, bundle: Bundle?)

Returns an `NSNib` object initialized to the nib file in the specified bundle.

typealias Name

