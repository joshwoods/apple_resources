

- Foundation
- NSKeyedArchiverDelegate
-  archiverWillFinish(\_:) 

Instance Method

# archiverWillFinish(\_:)

Notifies the delegate that encoding is about to finish.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func archiverWillFinish(_ archiver: NSKeyedArchiver)
```

## Parameters 

`archiver`  

The archiver that sent the message.

## See Also

### Encoding Data and Objects

func archiver(NSKeyedArchiver, didEncode: Any?)

Informs the delegate that a given object has been encoded.

func archiverDidFinish(NSKeyedArchiver)

Notifies the delegate that encoding has finished.

func archiver(NSKeyedArchiver, willEncode: Any) -> Any?

Informs the delegate that `object` is about to be encoded.

func archiver(NSKeyedArchiver, willReplace: Any?, with: Any?)

Informs the delegate that one given object is being substituted for another given object.

