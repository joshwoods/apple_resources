

- Core Image
- CIFilter
-  User Interface Options 

API Collection

# User Interface Options

Keys or values for the size of the input parameter controls for a filter view.

## Topics

### Constants

let IKUISizeFlavor: String

A key for the size of the controls in a filter view. The associated value can be IKUISizeMini, IKUISizeSmall, or IKUISizeRegular.

let IKUISizeMini: String

A very small control.

let IKUISizeSmall: String

A small control.

let IKUISizeRegular: String

A standard size control.

let IKUImaxSize: String

The maximum size of a filter view.

let IKUIFlavorAllowFallback: String

Substitute controls of another size. The associated value is a Boolean value. If the filter cannot provide a view for the requested size and a fallback is allowed, the filter can use controls of a different size.

