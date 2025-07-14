

- Foundation
-  NSValue 

Class

# NSValue

A simple container for a single C or Objective-C data item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSValue
```

## Overview

An NSValue object can hold any of the scalar types such as `int`, `float`, and `char`, as well as pointers, structures, and object `id` references. Use this class to work with such data types in collections (such as NSArray and NSSet), Key-value coding, and other APIs that require Objective-C objects. NSValue objects are always immutable.

### Subclassing Notes

The abstract NSValue class is the public interface of a class cluster consisting mostly of private, concrete classes that create and return a value object appropriate for a given situation. It is possible to subclass NSValue, but doing so requires providing storage facilities for the value (which is not inherited by subclasses) and implementing two primitive methods.

#### Methods to Override

Any subclass of NSValue *must* override the primitive instance methods getValue(_:) and objCType. These methods must operate on the storage that you provide for the value.

You might want to implement an initializer for your subclass that is suited to the storage you provide. The NSValue class does not have a designated initializer, so your initializer need only invoke the init() method of `super`. The NSValue class adopts the NSCopying and NSSecureCoding protocols; if you want instances of your own custom subclass created from copying or coding, override the methods in these protocols.

You may also wish to implement the hash method to make your subclass work well in collections.

#### Alternatives to Subclassing

If you need only to use NSValue objects for wrap a custom data types or structures defined by your app, you need not create an NSValue subclass. Instead, create a category that uses existing NSValue methods to store and retrieve data of your custom type. For example, the code below defines a custom Polyhedron structure and creates NSValue convenience methods to store and retrieve it:

```
typedef struct {
    int numFaces;
    float radius;
} Polyhedron;

@interface NSValue (Polyhedron)
+ (instancetype)valuewithPolyhedron:(Polyhedron)value;
@property (readonly) Polyhedron polyhedronValue;
@end

@implementation NSValue (Polyhedron)
+ (instancetype)valuewithPolyhedron:(Polyhedron)value
{
    return [self valueWithBytes:&value objCType:@encode(Polyhedron)];
}
- (Polyhedron) polyhedronValue
{
    Polyhedron value;
    [self getValue:&value];
    return value;
}
@end
```

## Topics

### Working with Raw Values

init(bytes: UnsafeRawPointer, objCType: UnsafePointer&lt;CChar>)

Initializes a value object to contain the specified value, interpreted with the specified Objective-C type.

init(UnsafeRawPointer, withObjCType: UnsafePointer&lt;CChar>)

Creates a value object containing the specified value, interpreted with the specified Objective-C type.

func getValue(UnsafeMutableRawPointer)

Copies the value into the specified buffer.

var objCType: UnsafePointer&lt;CChar>

A C string containing the Objective-C type of the data contained in the value object.

### Working with Pointer and Object Values

init(pointer: UnsafeRawPointer?)

Creates a value object containing the specified pointer.

init(nonretainedObject: Any?)

Creates a value object containing the specified object.

var pointerValue: UnsafeMutableRawPointer?

Returns the value as an untyped pointer.

var nonretainedObjectValue: Any?

The value as a non-retained pointer to an object.

### Working with Range Values

init(range: NSRange)

Creates a new value object containing the specified Foundation range structure.

var rangeValue: NSRange

The Foundation range structure representation of the value.

### Working with Foundation Geometry Values

init(point: NSPoint)

Creates a new value object containing the specified Foundation point structure.

init(size: NSSize)

Creates a new value object containing the specified Foundation size structure.

init(rect: NSRect)

Creates a new value object containing the specified Foundation rectangle structure.

var pointValue: NSPoint

The Foundation point structure representation of the value.

var sizeValue: NSSize

The Foundation size structure representation of the value.

var rectValue: NSRect

The Foundation rectangle structure representation of the value.

### Working with CoreGraphics Geometry Values

init(CGPoint: CGPoint)

Creates a new value object containing the specified CoreGraphics point structure.

init(CGVector: CGVector)

Creates a new value object containing the specified CoreGraphics vector structure.

init(CGSize: CGSize)

Creates a new value object containing the specified CoreGraphics size structure.

init(CGRect: CGRect)

Creates a new value object containing the specified CoreGraphics rectangle structure.

init(CGAffineTransform: CGAffineTransform)

Creates a new value object containing the specified CoreGraphics affine transform structure.

var cgPointValue: CGPoint

Returns the CoreGraphics point structure representation of the value.

var cgVectorValue: CGVector

Returns the CoreGraphics vector structure representation of the value.

var cgSizeValue: CGSize

Returns the CoreGraphics size structure representation of the value.

var cgRectValue: CGRect

Returns the CoreGraphics rectangle structure representation of the value.

var cgAffineTransformValue: CGAffineTransform

Returns the CoreGraphics affine transform representation of the value.

### Working with UIKit Geometry Values

init(UIEdgeInsets: UIEdgeInsets)

Creates a new value object containing the specified UIKit edge insets structure.

init(UIOffset: UIOffset)

Creates a new value object containing the specified UIKit offset structure.

var uiEdgeInsetsValue: UIEdgeInsets

Returns the UIKit edge insets structure representation of the value.

var uiOffsetValue: UIOffset

Returns the UIKit offset structure representation of the value.

### Working with CoreAnimation Transform Values

init(CATransform3D: CATransform3D)

Creates a new value object containing the specified CoreAnimation transform structure.

var caTransform3DValue: CATransform3D

The CoreAnimation transform structure representation of the value.

### Working with Media Time Values

init(CMTime: CMTime)

Creates a new value object containing the specified CoreMedia time structure.

init(CMTimeRange: CMTimeRange)

Creates a new value object containing the specified CoreMedia time range structure.

init(CMTimeMapping: CMTimeMapping)

Creates a new value object containing the specified CoreMedia time mapping structure.

var timeValue: CMTime

The CoreMedia time structure representation of the value.

var timeRangeValue: CMTimeRange

The CoreMedia time range structure representation of the value.

var timeMappingValue: CMTimeMapping

The CoreMedia time mapping structure representation of the value.

### Working with Geographic Coordinate Values

init(MKCoordinate: CLLocationCoordinate2D)

Creates a new value object containing the specified CoreLocation geographic coordinate structure.

init(MKCoordinateSpan: MKCoordinateSpan)

Creates a new value object containing the specified MapKit coordinate span structure.

var mkCoordinateValue: CLLocationCoordinate2D

The CoreLocation geographic coordinate structure representation of the value.

var mkCoordinateSpanValue: MKCoordinateSpan

The MapKit coordinate span structure representation of the value.

### Working with SceneKit Vector and Matrix Values

init(SCNVector3: SCNVector3)

Creates a value object that contains the specified three-element SceneKit vector.

init(SCNVector4: SCNVector4)

Creates a value object that contains the specified four-element SceneKit vector.

init(SCNMatrix4: SCNMatrix4)

Creates a value object that contains the specified SceneKit 4 x 4 matrix.

var scnVector3Value: SCNVector3

The three-element Scene Kit vector representation of the value.

var scnVector4Value: SCNVector4

The four-element Scene Kit vector representation of the value.

var scnMatrix4Value: SCNMatrix4

The Scene Kit 4 x 4 matrix representation of the value.

### Comparing Value Objects

func isEqual(to: NSValue) -> Bool

Returns a Boolean value that indicates whether the value object and another value object are equal.

### Initializers

init!(CMVideoDimensions: CMVideoDimensions)

convenience init(GCPoint2: GCPoint2)

init?(coder: NSCoder)

init(directionalEdgeInsets: NSDirectionalEdgeInsets)

init(edgeInsets: NSEdgeInsets)

### Instance Properties

var directionalEdgeInsetsValue: NSDirectionalEdgeInsets

var edgeInsetsValue: NSEdgeInsets

var gcPoint2Value: GCPoint2

var videoDimensionsValue: CMVideoDimensions

### Instance Methods

func getValue(UnsafeMutableRawPointer, size: Int)

func value&lt;StoredType>(of: StoredType.Type) -> StoredType?

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSNumber

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Value Wrappers and Transformations

class NSNumber

An object wrapper for primitive scalar numeric values.

class ValueTransformer

An abstract class used to transform values from one representation to another.

