

- AppKit
- NSViewController
-  nibName 

Instance Property

# nibName

The name of the nib file to be loaded to instantiate the receiver’s primary view.

macOS 10.5+

``` source
@MainActor
var nibName: NSNib.Name? { get }
```

## Discussion

This property’s value is the name you provide to the `nibNameOrNil` parameter in the init(nibName:bundle:) method.

## See Also

### Related Documentation

init(nibName: NSNib.Name?, bundle: Bundle?)

Returns a view controller object initialized to the nib file in the specified bundle.

### Nib Properties

var nibBundle: Bundle?

The nib bundle to be loaded to instantiate the receiver’s primary view.

