

- Paravirtualized Graphics
- PGDisplayDescriptor
-  sizeInMillimeters 

Instance Property

# sizeInMillimeters

The size in millimeters of the virtual display.

Mac Catalyst 14.0+macOS 11.0+

``` source
var sizeInMillimeters: NSSize { get set }
```

## Discussion

The device propagates the display size to the guest operating system. The app can scale the resulting screen data to a different size in its user interface.

## See Also

### Specifying the Display Properties

var name: String?

The display’s name as seen in the guest operating environment.

