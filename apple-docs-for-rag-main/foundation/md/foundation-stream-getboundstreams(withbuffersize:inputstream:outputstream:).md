

- Foundation
- Stream
-  getBoundStreams(withBufferSize:inputStream:outputStream:) 

Type Method

# getBoundStreams(withBufferSize:inputStream:outputStream:)

Creates and returns by reference a bound pair of input and output streams.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func getBoundStreams(
    withBufferSize bufferSize: Int,
    inputStream: AutoreleasingUnsafeMutablePointer?,
    outputStream: AutoreleasingUnsafeMutablePointer?
)
```

## Parameters 

`bufferSize`  

The size of the buffer, in bytes, used to transfer data from `inputStream` to `outputStream`.

`inputStream`  

On return, contains an input stream.

`outputStream`  

On return, contains an output stream.

## Mentioned in 

Uploading streams of data

## Discussion

The created streams are bound to one another, such that any data written to `outputStream` is received by `inputStream`.

This is a convenience method for calling CFStreamCreateBoundPair(_:_:_:_:) and bridging from the returned Core Foundation types.

## See Also

### Related Documentation

func CFStreamCreateBoundPair(_ alloc: CFAllocator!, _ readStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, _ writeStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!, _ transferBufferSize: CFIndex)

Creates a bound pair of read and write streams.

