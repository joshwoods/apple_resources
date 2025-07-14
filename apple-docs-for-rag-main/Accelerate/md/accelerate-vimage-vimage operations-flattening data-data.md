

- Accelerate
- vImage
- vImage Operations
-  Flattening data 

API Collection

# Flattening data

Perform an alpha composite of a four-channel image over a solid background color.

## Topics

### Flattening 4-channel, 8-bit images

func vImageFlatten_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of an 8-bit-per-channel, 4-channel ARGB buffer over a solid background color.

func vImageFlatten_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of an 8-bit-per-channel, 4-channel RGBA buffer over a solid background color.

### Flattening 4-channel, 8-bit images to three channels

func vImageFlatten_ARGB8888ToRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, Bool, vImage_Flags) -> vImage_Error

Flattens an 8-bit-per-channel ARGB buffer against a solid background to produce an 8-bit-per-channel RGB result.

func vImageFlatten_BGRA8888ToRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, Bool, vImage_Flags) -> vImage_Error

Flattens an 8-bit-per-channel BGRA buffer against a solid background to produce an 8-bit-per-channel RGB result.

vImageFlatten_BGRA8888ToBGR888

Flattens an 8-bit-per-channel BGRA buffer against a solid background to produce an 8-bit-per-channel BGR result.

func vImageFlatten_RGBA8888ToRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, Bool, vImage_Flags) -> vImage_Error

Flattens an 8-bit-per-channel RGBA buffer against a solid background to produce an 8-bit-per-channel RGB result.

vImageFlatten_RGBA8888ToBGR888

Flattens an 8-bit-per-channel RGBA buffer against a solid background to produce an 8-bit-per-channel BGR result.

### Flattening 4-channel,16-bit images

func vImageFlatten_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt16>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of an unsigned 16-bit-per-channel, 4-channel ARGB buffer over a solid background color.

func vImageFlatten_RGBA16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt16>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of an unsigned 16-bit-per-channel, 4-channel RGBA buffer over a solid background color.

func vImageFlatten_RGBA16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Int16>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of a fixed-point 16-bit-per-channel, 4-channel RGBA buffer over a solid background color.

func vImageFlatten_ARGB16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Int16>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of a fixed-point 16-bit-per-channel, 4-channel ARGB buffer over a solid background color.

### Flattening 4-channel, 32-bit images

func vImageFlatten_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of a 32-bit-per-channel, 4-channel ARGB buffer over a solid background color.

func vImageFlatten_RGBAFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of a 32-bit-per-channel, 4-channel RGBA buffer over a solid background color.

### Flattening 4-channel, 32-bit images to three channels

func vImageFlatten_ARGBFFFFToRGBFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, Bool, vImage_Flags) -> vImage_Error

Flattens a 32-bit-per-channel ARGB buffer against a solid background to produce a 32-bit-per-channel RGB result.

func vImageFlatten_BGRAFFFFToRGBFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, Bool, vImage_Flags) -> vImage_Error

Flattens a 32-bit-per-channel BGRA buffer against a solid background to produce a 32-bit-per-channel RGB result.

func vImageFlatten_RGBAFFFFToRGBFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, Bool, vImage_Flags) -> vImage_Error

Flattens a 32-bit-per-channel RGBA buffer against a solid background to produce a 32-bit-per-channel RGB result.

