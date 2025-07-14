

- Paravirtualized Graphics
- PGDisplayDescriptor
-  name 

Instance Property

# name

The display’s name as seen in the guest operating environment.

Mac Catalyst 14.0+macOS 11.0+

``` source
var name: String? { get set }
```

## Discussion

The default value is `Apple Virtual`. The framework truncates the name to 13 characters.

The device propagates the display name into the guest environment, so the name may be visible in the guest operating system’s user interface.

## See Also

### Specifying the Display Properties

var sizeInMillimeters: NSSize

The size in millimeters of the virtual display.

