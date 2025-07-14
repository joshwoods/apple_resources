

- Dispatch
- DispatchData
-  copyBytes(to:from:) 

Instance Method

# copyBytes(to:from:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwiftDeprecated

``` source
func copyBytes(
    to pointer: UnsafeMutablePointer,
    from range: Range
)
```

## See Also

### Combining Sequence Elements

func append(DispatchData)

func append&lt;SourceType>(UnsafeBufferPointer&lt;SourceType>)

func append(UnsafeRawBufferPointer)

func append(UnsafePointer&lt;UInt8>, count: Int)

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, count: Int)

func copyBytes(to: UnsafeMutableRawBufferPointer, count: Int)

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: Range&lt;DispatchData.Index>?) -> Int

func copyBytes(to: UnsafeMutableRawBufferPointer, from: Range&lt;DispatchData.Index>)

func enumerateBytes((UnsafeBufferPointer&lt;UInt8>, Int, inout Bool) -> Void)

func makeIterator() -> DispatchData.Iterator

func region(location: Int) -> (data: DispatchData, offset: Int)

func subdata(in: Range&lt;DispatchData.Index>) -> DispatchData

func withUnsafeBytes&lt;Result, ContentType>(body: (UnsafePointer&lt;ContentType>) throws -> Result) rethrows -> Result

