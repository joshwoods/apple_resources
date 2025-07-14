

- Foundation
-  NSKeyedUnarchiverDelegate 

Protocol

# NSKeyedUnarchiverDelegate

The optional methods implemented by the delegate of a keyed unarchiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSKeyedUnarchiverDelegate : NSObjectProtocol
```

## Topics

### Decoding Objects

func unarchiver(NSKeyedUnarchiver, cannotDecodeObjectOfClassName: String, originalClasses: [String]) -> AnyClass?

Informs the delegate that the class with a given name is not available during decoding.

func unarchiver(NSKeyedUnarchiver, didDecode: Any?) -> Any?

Informs the delegate that a given object has been decoded.

func unarchiver(NSKeyedUnarchiver, willReplace: Any, with: Any)

Informs the delegate that one object is being substituted for another.

### Finishing Decoding

func unarchiverDidFinish(NSKeyedUnarchiver)

Notifies the delegate that decoding has finished.

func unarchiverWillFinish(NSKeyedUnarchiver)

Notifies the delegate that decoding is about to finish.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Keyed Archivers

class NSKeyedArchiver

An encoder that stores an object’s data to an archive referenced by keys.

protocol NSKeyedArchiverDelegate

The optional methods implemented by the delegate of a keyed archiver.

class NSKeyedUnarchiver

A decoder that restores data from an archive referenced by keys.

class NSCoder

An abstract class that serves as the basis for objects that enable archiving and distribution of other objects.

class NSSecureUnarchiveFromDataTransformer

A value transformer that converts data to and from classes that support secure coding.

