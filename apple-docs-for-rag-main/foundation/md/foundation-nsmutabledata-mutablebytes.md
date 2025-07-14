

- Foundation
- NSMutableData
-  mutableBytes 

Instance Property

# mutableBytes

A pointer to the data contained by the mutable data object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var mutableBytes: UnsafeMutableRawPointer { get }
```

## Discussion

If the length of the receiver’s data is not zero, this property is guaranteed to contain a pointer to the object’s internal bytes. If the length of receiver’s data *is* zero, this property may or may not contain `NULL` dependent upon many factors related to how the object was created (moreover, in this case the method result might change between different releases). The returned pointer is valid until the data object is deallocated.

Note

This property is similar to, but different than the bytes property. The bytes property contains a pointer to a constant. You can use The bytes pointer to read the data managed by the data object, but you cannot modify that data. However, if the mutableBytes property contains a non-`null` pointer, this pointer points to mutable data. You can use the mutableBytes pointer to modify the data managed by the data object.

A sample using this method can be found in Working With Mutable Binary Data.

## See Also

### Related Documentation

var bytes: UnsafeRawPointer

A pointer to the data object’s contents.

