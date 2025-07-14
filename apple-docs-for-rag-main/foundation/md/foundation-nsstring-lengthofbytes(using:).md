

- Foundation
- NSString
-  lengthOfBytes(using:) 

Instance Method

# lengthOfBytes(using:)

Returns the number of bytes required to store the receiver in a given encoding.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func lengthOfBytes(using enc: UInt) -> Int
```

## Parameters 

`enc`  

The encoding for which to determine the receiver’s length.

## Return Value

The number of bytes required to store the receiver in the encoding `enc` in a non-external representation. The length does not include space for a terminating `NULL` character. Returns `0` if the specified encoding cannot be used to convert the receiver or if the amount of memory required for storing the results of the encoding conversion would exceed NSIntegerMax.

## Discussion

The result is exact and is returned in `O(n)` time.

## See Also

### Getting a String’s Length

var length: Int

The number of UTF-16 code units in the receiver.

func maximumLengthOfBytes(using: UInt) -> Int

Returns the maximum number of bytes needed to store the receiver in a given encoding.

