

- Kernel
- Kernel Data Types
- twolevel_hint
-  isub_image 

Instance Property

# isub_image

The subimage in which the symbol is defined. It is an index into the list of images that make up the umbrella image. If this field is 0, the symbol is in the umbrella image itself. If the image is not an umbrella framework or library, this field is 0.

macOS 10.6+

``` source
uint32_t isub_image:8;
```

