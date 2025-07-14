

- AppKit
- NSSharingService
-  delegate 

Instance Property

# delegate

Specifies the delegate of the sharing service.

macOS 10.8+

``` source
weak var delegate: (any NSSharingServiceDelegate)? { get set }
```

## Discussion

The delegate class must conform to the NSSharingServiceDelegate protocol.

## See Also

### Managing the Delegate

protocol NSSharingServiceDelegate

A set of methods that you use to customize the position and animation of a share sheet, and to be notified whether the item is successfully shared.

