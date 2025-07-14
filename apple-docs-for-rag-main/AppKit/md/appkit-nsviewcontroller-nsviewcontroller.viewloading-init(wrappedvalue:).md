

- AppKit
- NSViewController
- NSViewController.ViewLoading
-  init(wrappedValue:) 

Initializer

# init(wrappedValue:)

Creates a property wrapper that loads the view controller’s view before accessing the property.

macOS 13.3+Swift 5.1+

``` source
init(wrappedValue: Value)
```

## Parameters 

`wrappedValue`  

The underlying value tied to the loading of the view.

## See Also

### Creating a ViewLoading Property Wrapper

init()

Creates an empty property wrapper that loads the view controller’s view before accessing the property.

