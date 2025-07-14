

- Foundation
-  NSKeyedArchiverDelegate 

Protocol

# NSKeyedArchiverDelegate

The optional methods implemented by the delegate of a keyed archiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSKeyedArchiverDelegate : NSObjectProtocol
```

## Topics

### Encoding Data and Objects

func archiver(NSKeyedArchiver, didEncode: Any?)

Informs the delegate that a given object has been encoded.

func archiverDidFinish(NSKeyedArchiver)

Notifies the delegate that encoding has finished.

func archiver(NSKeyedArchiver, willEncode: Any) -> Any?

Informs the delegate that `object` is about to be encoded.

func archiverWillFinish(NSKeyedArchiver)

Notifies the delegate that encoding is about to finish.

func archiver(NSKeyedArchiver, willReplace: Any?, with: Any?)

Informs the delegate that one given object is being substituted for another given object.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Keyed Archivers

class NSKeyedArchiver

An encoder that stores an object’s data to an archive referenced by keys.

class NSKeyedUnarchiver

A decoder that restores data from an archive referenced by keys.

protocol NSKeyedUnarchiverDelegate

The optional methods implemented by the delegate of a keyed unarchiver.

class NSCoder

An abstract class that serves as the basis for objects that enable archiving and distribution of other objects.

class NSSecureUnarchiveFromDataTransformer

A value transformer that converts data to and from classes that support secure coding.

