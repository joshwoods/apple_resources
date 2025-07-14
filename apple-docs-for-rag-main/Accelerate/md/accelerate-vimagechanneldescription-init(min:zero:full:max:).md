

- Accelerate
- vImageChannelDescription
-  init(min:zero:full:max:) 

Initializer

# init(min:zero:full:max:)

Returns a structure that describes the range and clamp limits for a pixel format.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    min: CGFloat,
    zero: CGFloat,
    full: CGFloat,
    max: CGFloat
)
```

## Parameters 

`min`  

The minimum encoded value.

`zero`  

The encoding for the value `0.0`.

`full`  

The encoding for `1.0` (`0.5` for chrominance).

`max`  

The maximum encoded value.

## Return Value

A structure that describes the range and clamp limits for a pixel format.

## See Also

### Creating a channel description

init()

Returns an empty structure that describes the range and clamp limits for a pixel format.

