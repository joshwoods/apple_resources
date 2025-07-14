

- RealityKit
- LowLevelMesh
-  withUnsafeIndices(\_:) 

Instance Method

# withUnsafeIndices(\_:)

Reads the index buffer synchronously on the CPU.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func withUnsafeIndices(_ callback: (UnsafeRawBufferPointer) -> Void)
```

## Discussion

The buffer is only valid for the lifetime of the callback.

## See Also

### Accessing mesh data on the CPU with Swift

func withUnsafeBytes(bufferIndex: Int, (UnsafeRawBufferPointer) -> Void)

Reads a Metal vertex buffer synchronously on the CPU.

func withUnsafeMutableBytes(bufferIndex: Int, (UnsafeMutableRawBufferPointer) -> Void)

Updates a Metal vertex buffer synchronously on the CPU.

func withUnsafeMutableIndices((UnsafeMutableRawBufferPointer) -> Void)

Updates the index buffer synchronously on the CPU.

func replaceUnsafeMutableBytes(bufferIndex: Int, (UnsafeMutableRawBufferPointer) -> Void)

Replaces a Metal vertex buffer synchronously on the CPU.

func replaceUnsafeMutableIndices((UnsafeMutableRawBufferPointer) -> Void)

Replaces the index buffer synchronously on the CPU.

