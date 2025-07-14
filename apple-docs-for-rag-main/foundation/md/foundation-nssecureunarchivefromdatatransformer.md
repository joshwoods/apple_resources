

- Foundation
-  NSSecureUnarchiveFromDataTransformer 

Class

# NSSecureUnarchiveFromDataTransformer

A value transformer that converts data to and from classes that support secure coding.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class NSSecureUnarchiveFromDataTransformer
```

## Overview

This class provides a default ValueTransformer implementation for secure decoding. This class attempts to decode data into the classes listed within allowedTopLevelClasses, which includes NSArray, NSDictionary, NSSet, NSString, NSNumber, NSDate, NSData, NSURL, NSUUID, and NSNull.

To archive or unarchive other classes that support NSSecureCoding, create a subclass and override allowedTopLevelClasses to list the classes to transform.

To use NSSecureUnarchiveFromDataTransformer with Core Data, use the name of this class, or the name of a subclass you implement, as the name of the transformer for an entity’s attribute within a Core Data Model. If you use your own transformer subclass, register it with your app before intializing your persistent container with Core Data.

For an example of subclassing NSSecureUnarchiveFromDataTransformer, see Handling Different Data Types in Core Data, which has a `ColorToDataTransformer` class that transforms UIColor to NSData and the reverse, to support archiving instances of UIColor.

## Topics

### Getting Information About a Transformer

class var allowedTopLevelClasses: [AnyClass]

A list of allowed classes the top-level object in an archive must conform to, for encoding and decoding.

## Relationships

### Inherits From

- ValueTransformer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Keyed Archivers

class NSKeyedArchiver

An encoder that stores an object’s data to an archive referenced by keys.

protocol NSKeyedArchiverDelegate

The optional methods implemented by the delegate of a keyed archiver.

class NSKeyedUnarchiver

A decoder that restores data from an archive referenced by keys.

protocol NSKeyedUnarchiverDelegate

The optional methods implemented by the delegate of a keyed unarchiver.

class NSCoder

An abstract class that serves as the basis for objects that enable archiving and distribution of other objects.

