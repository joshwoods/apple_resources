

- Core Graphics
- CGColorConversionInfo
-  convert(width:height:to:format:from:format:options:) 

Instance Method

# convert(width:height:to:format:from:format:options:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func convert(
    width: Int,
    height: Int,
    to dst_data: UnsafeMutableRawPointer,
    format dst_format: CGColorBufferFormat,
    from src_data: UnsafeRawPointer,
    format src_format: CGColorBufferFormat,
    options: CFDictionary?
) -> Bool
```

