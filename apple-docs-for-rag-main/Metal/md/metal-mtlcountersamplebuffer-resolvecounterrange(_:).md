

- Metal
- MTLCounterSampleBuffer
-  resolveCounterRange(\_:) 

Instance Method

# resolveCounterRange(\_:)

Transforms samples of a GPU’s counter set from the driver’s internal format to a standard Metal data structure.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOS

``` source
func resolveCounterRange(_ range: Range) throws -> Data?
```

## Parameters 

`range`  

A range that indicates which sample instances the method resolves in the counter sample buffer.

## Return Value

A Data instance in Swift, or an NSData instance in Objective-C, if the method successfully resolves the range of samples in the buffer; otherwise, `nil`.

## Mentioned in 

Converting a GPU’s Counter Data into a Readable Format

## Discussion

You can only call this method on a counter sample buffer that you create with MTLStorageMode.shared (see storageMode). For an example of how and when to use this method, see Converting a GPU’s Counter Data into a Readable Format.

Note

The GPU stores MTLCounterErrorValue in `destinationBuffer` each time it encounters an error resolving a sample.

