

- Foundation
- NSData
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Returns a Boolean value indicating whether this data object is the same as another.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(to other: Data) -> Bool
```

## Parameters 

`other`  

The data object with which to compare the receiver.

## Return Value

true if the contents of `otherData` are equal to the contents of the receiver, otherwise false.

## Discussion

Two data objects are equal if they hold the same number of bytes, and if the bytes at the same position in the objects are the same.

## See Also

### Testing Data

var length: Int

The number of bytes contained by the data object.

