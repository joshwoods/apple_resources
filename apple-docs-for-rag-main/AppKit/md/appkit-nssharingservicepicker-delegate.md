

- AppKit
- NSSharingServicePicker
-  delegate 

Instance Property

# delegate

The object for managing the sharing service picker.

macOS 10.8+

``` source
weak var delegate: (any NSSharingServicePickerDelegate)? { get set }
```

## Discussion

The delegate object must conform to the NSSharingServicePickerDelegate delegate.

## See Also

### Managing the sharing service picker

protocol NSSharingServicePickerDelegate

An interface for managing content for the macOS share sheet.

