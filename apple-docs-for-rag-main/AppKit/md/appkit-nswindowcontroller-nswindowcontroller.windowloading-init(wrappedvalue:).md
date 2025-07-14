

- AppKit
- NSWindowController
- NSWindowController.WindowLoading
-  init(wrappedValue:) 

Initializer

# init(wrappedValue:)

Creates a property wrapper that loads the window controller’s window before accessing the property.

macOS 13.3+Swift 5.1+

``` source
init(wrappedValue: Value)
```

## Parameters 

`wrappedValue`  

The underlying value tied to the loading of the window.

## See Also

### Creating a WindowLoading Property Wrapper

init()

Creates an empty property wrapper that loads the window controller’s window before accessing the property.

