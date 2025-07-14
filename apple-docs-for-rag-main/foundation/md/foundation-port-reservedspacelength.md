

- Foundation
- Port
-  reservedSpaceLength 

Instance Property

# reservedSpaceLength

The number of bytes of space reserved by the receiver for sending data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var reservedSpaceLength: Int { get }
```

## Discussion

The number of bytes reserved by the receiver for sending data. The default length is `0`.

## See Also

### Setting Information

func send(before: Date, components: NSMutableArray?, from: Port?, reserved: Int) -> Bool

This method is provided for subclasses that have custom types of `NSPort`.

func send(before: Date, msgid: Int, components: NSMutableArray?, from: Port?, reserved: Int) -> Bool

This method is provided for subclasses that have custom types of `NSPort`.

