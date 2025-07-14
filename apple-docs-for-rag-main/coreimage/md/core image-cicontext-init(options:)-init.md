

- Core Image
- CIContext
-  init(options:) 

Initializer

# init(options:)

Initializes a context without a specific rendering destination, using the specified options.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init(options: [CIContextOption : Any]? = nil)
```

## Parameters 

`options`  

A dictionary containing options for the context. For applicable keys and values, see `Context Options`.

## Return Value

An initialized Core Image context.

## Discussion

If you create a context without specifying a rendering destination, Core Image automatically chooses and internally manages a rendering destination based on the current device’s capabilities and your settings in the `options` dictionary. You cannot use a context without an explicit destination for the methods listed in Drawing Images. Instead, use the methods listed in Rendering Images.

The `options` dictionary defines behaviors for the context, such as color space and rendering quality. For example, to create a CPU-based context, use the useSoftwareRenderer key.

## See Also

### Creating a Context Without Specifying a Destination

init()

Initializes a context without a specific rendering destination, using default options.

