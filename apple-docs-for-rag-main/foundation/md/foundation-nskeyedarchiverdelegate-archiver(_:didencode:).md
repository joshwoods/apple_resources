

- Foundation
- NSKeyedArchiverDelegate
-  archiver(\_:didEncode:) 

Instance Method

# archiver(\_:didEncode:)

Informs the delegate that a given object has been encoded.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func archiver(
    _ archiver: NSKeyedArchiver,
    didEncode object: Any?
)
```

## Parameters 

`archiver`  

The archiver that sent the message.

`object`  

The object that has been encoded. `object` may be `nil`.

## Discussion

The delegate might restore some state it had modified previously, or use this opportunity to keep track of the objects that are encoded.

This method is not called for conditional objects until they are actually encoded (if ever).

## See Also

### Related Documentation

Archives and Serializations Programming Guide

### Encoding Data and Objects

func archiverDidFinish(NSKeyedArchiver)

Notifies the delegate that encoding has finished.

func archiver(NSKeyedArchiver, willEncode: Any) -> Any?

Informs the delegate that `object` is about to be encoded.

func archiverWillFinish(NSKeyedArchiver)

Notifies the delegate that encoding is about to finish.

func archiver(NSKeyedArchiver, willReplace: Any?, with: Any?)

Informs the delegate that one given object is being substituted for another given object.

