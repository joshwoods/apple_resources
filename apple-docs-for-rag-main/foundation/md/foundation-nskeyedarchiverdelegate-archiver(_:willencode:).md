

- Foundation
- NSKeyedArchiverDelegate
-  archiver(\_:willEncode:) 

Instance Method

# archiver(\_:willEncode:)

Informs the delegate that `object` is about to be encoded.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func archiver(
    _ archiver: NSKeyedArchiver,
    willEncode object: Any
) -> Any?
```

## Parameters 

`archiver`  

The archiver that sent the message.

`object`  

The object that is about to be encoded. This value is never `nil`.

## Return Value

Either `object` or a different object to be encoded in its stead. The delegate can also modify the coder state. If the delegate returns `nil`, `nil` is encoded.

## Discussion

This method is called after the original object may have replaced itself with replacementObject(for:):.

This method is called whether or not the object is being encoded conditionally.

This method is not called for an object once a replacement mapping has been set up for that object (either explicitly, or because the object has previously been encoded). This method is also not called when `nil` is about to be encoded.

## See Also

### Encoding Data and Objects

func archiver(NSKeyedArchiver, didEncode: Any?)

Informs the delegate that a given object has been encoded.

func archiverDidFinish(NSKeyedArchiver)

Notifies the delegate that encoding has finished.

func archiverWillFinish(NSKeyedArchiver)

Notifies the delegate that encoding is about to finish.

func archiver(NSKeyedArchiver, willReplace: Any?, with: Any?)

Informs the delegate that one given object is being substituted for another given object.

