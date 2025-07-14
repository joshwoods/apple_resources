

- Core Image
- CIContext
-  init() 

Initializer

# init()

Initializes a context without a specific rendering destination, using default options.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init()
```

## Return Value

An initialized Core Image context.

## Discussion

If you create a context without specifying a rendering destination, Core Image automatically chooses and internally manages a rendering destination based on the current device’s capabilities. You cannot use a context without an explicit destination for the methods listed in Drawing Images. Instead, use the methods listed in Rendering Images.

To specify additional options for the context, use the init(options:) initializer instead.

## See Also

### Creating a Context Without Specifying a Destination

init(options: [CIContextOption : Any]?)

Initializes a context without a specific rendering destination, using the specified options.

