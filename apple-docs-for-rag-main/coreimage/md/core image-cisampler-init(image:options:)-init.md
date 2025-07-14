

- Core Image
- CISampler
-  init(image:options:) 

Initializer

# init(image:options:)

Initializes the sampler with an image object using options specified in a dictionary.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init(
    image im: CIImage,
    options dict: [AnyHashable : Any]? = nil
)
```

## Parameters 

`im`  

The image to initialize the sampler with.

`dict`  

A dictionary that contains options specified as key-value pairs. See Sampler Option Keys.

## See Also

### Initializing a Sampler

init(image: CIImage)

Initializes a sampler with an image object.

### Related Documentation

- initWithImage:keysAndValues:

Initializes the sampler with an image object using options specified as key-value pairs.

