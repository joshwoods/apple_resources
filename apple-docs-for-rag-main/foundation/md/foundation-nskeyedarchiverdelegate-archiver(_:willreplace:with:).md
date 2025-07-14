

- Foundation
- NSKeyedArchiverDelegate
-  archiver(\_:willReplace:with:) 

Instance Method

# archiver(\_:willReplace:with:)

Informs the delegate that one given object is being substituted for another given object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func archiver(
    _ archiver: NSKeyedArchiver,
    willReplace object: Any?,
    with newObject: Any?
)
```

## Parameters 

`archiver`  

The archiver that sent the message.

`object`  

The object being replaced in the archive.

`newObject`  

The object replacing `object` in the archive.

## Discussion

This method is called even when the delegate itself is doing, or has done, the substitution. The delegate may use this method if it is keeping track of the encoded or decoded objects.

## See Also

### Encoding Data and Objects

func archiver(NSKeyedArchiver, didEncode: Any?)

Informs the delegate that a given object has been encoded.

func archiverDidFinish(NSKeyedArchiver)

Notifies the delegate that encoding has finished.

func archiver(NSKeyedArchiver, willEncode: Any) -> Any?

Informs the delegate that `object` is about to be encoded.

func archiverWillFinish(NSKeyedArchiver)

Notifies the delegate that encoding is about to finish.

