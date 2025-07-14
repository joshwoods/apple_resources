

- Accelerate
-  vImageBuffer_GetSize(\_:) 

Function

# vImageBuffer_GetSize(\_:)

Returns the size, in pixels, of a vImage buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageBuffer_GetSize(_ buf: UnsafePointer) -> CGSize
```

## Parameters 

`buf`  

The vImage buffer to query.

## Return Value

The size of the buffer.

## Discussion

The vImage library defines a buffer’s width and height as vImagePixelCount values that may be larger than doc://com.apple.documentation/documentation/corefoundation/cgfloat/1845207-greatestfinitemagnitude. This function rounds down the buffer’s dimensions to the nearest representable CGFloat values that are less than, or equal to, the size of the buffer.

