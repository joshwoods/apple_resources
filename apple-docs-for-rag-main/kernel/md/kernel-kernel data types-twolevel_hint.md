

- Kernel
- Kernel Data Types
-  twolevel_hint 

# twolevel_hint

macOS 10.6+

``` source
struct twolevel_hint {
    ...
};
```

## Topics

### Instance Properties

isub_image

The subimage in which the symbol is defined. It is an index into the list of images that make up the umbrella image. If this field is 0, the symbol is in the umbrella image itself. If the image is not an umbrella framework or library, this field is 0.

itoc

The symbol index into the table of contents of the image specified by the `isub_image` field.

