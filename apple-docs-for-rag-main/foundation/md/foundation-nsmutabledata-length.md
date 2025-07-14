

- Foundation
- NSMutableData
-  length 

Instance Property

# length

The number of bytes contained in the mutable data object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var length: Int { get set }
```

## Discussion

The mutable data object’s length parameter is read-writeable. You can set this parameter to expand or truncate the number of bytes contained by the data object. If the mutable data object is expanded, the additional bytes are filled with zeros.

Important

Changing the length of a mutable data object invalidate any existing data pointers returned by the bytes or mutableBytes properties.

## See Also

### Related Documentation

func increaseLength(by: Int)

Increases the length of the receiver by a given number of bytes.

