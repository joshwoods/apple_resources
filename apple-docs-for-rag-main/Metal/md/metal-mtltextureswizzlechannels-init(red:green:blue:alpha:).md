

- Metal
- MTLTextureSwizzleChannels
-  init(red:green:blue:alpha:) 

Initializer

# init(red:green:blue:alpha:)

Creates a swizzle pattern.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
init(
    red: MTLTextureSwizzle,
    green: MTLTextureSwizzle,
    blue: MTLTextureSwizzle,
    alpha: MTLTextureSwizzle
)
```

## Parameters 

`red`  

The data you want to copy to the first output channel

`green`  

The data you want to copy to the second output channel

`blue`  

The data you want to copy to the third output channel

`alpha`  

The data you want to copy to the fourth output channel

## See Also

### Creating a Swizzle Pattern

init()

Creates a default swizzle pattern.

