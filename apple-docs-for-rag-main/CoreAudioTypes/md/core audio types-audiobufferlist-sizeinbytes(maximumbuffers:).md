

- Core Audio Types
- AudioBufferList
-  sizeInBytes(maximumBuffers:) 

Type Method

# sizeInBytes(maximumBuffers:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func sizeInBytes(maximumBuffers: Int) -> Int
```

## Return Value

The size in bytes of an `AudioBufferList` that can hold up to `maximumBuffers` `AudioBuffer`s.

