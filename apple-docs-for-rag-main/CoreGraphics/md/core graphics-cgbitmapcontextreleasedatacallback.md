

- Core Graphics
-  CGBitmapContextReleaseDataCallback 

Type Alias

# CGBitmapContextReleaseDataCallback

A callback function used to release data associate with the bitmap context.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGBitmapContextReleaseDataCallback = (UnsafeMutableRawPointer?, UnsafeMutableRawPointer?) -> Void
```

## Discussion

The `releaseInfo` parameter contains the contextual data that you passed to the init(data:width:height:bitsPerComponent:bytesPerRow:space:bitmapInfo:releaseCallback:releaseInfo:) function. The `data` parameter contains a pointer to the bitmap data for you to release.

## See Also

### Creating Bitmap Graphics Contexts

init?(data: UnsafeMutableRawPointer?, width: Int, height: Int, bitsPerComponent: Int, bytesPerRow: Int, space: CGColorSpace, bitmapInfo: UInt32)

Creates a bitmap graphics context.

init?(data: UnsafeMutableRawPointer?, width: Int, height: Int, bitsPerComponent: Int, bytesPerRow: Int, space: CGColorSpace, bitmapInfo: UInt32, releaseCallback: CGBitmapContextReleaseDataCallback?, releaseInfo: UnsafeMutableRawPointer?)

Creates a bitmap graphics context with the specified callback function.

