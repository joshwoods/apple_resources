

- AppKit
- NSViewController
-  nibBundle 

Instance Property

# nibBundle

The nib bundle to be loaded to instantiate the receiver’s primary view.

macOS 10.5+

``` source
@MainActor
var nibBundle: Bundle? { get }
```

## Discussion

This property’s value is the bundle you provide to the `nibBundleOrNil` parameter in the init(nibName:bundle:) method.

## See Also

### Nib Properties

var nibName: NSNib.Name?

The name of the nib file to be loaded to instantiate the receiver’s primary view.

