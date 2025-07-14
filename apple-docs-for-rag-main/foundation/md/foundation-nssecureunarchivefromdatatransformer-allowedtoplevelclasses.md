

- Foundation
- NSSecureUnarchiveFromDataTransformer
-  allowedTopLevelClasses 

Type Property

# allowedTopLevelClasses

A list of allowed classes the top-level object in an archive must conform to, for encoding and decoding.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class var allowedTopLevelClasses: [AnyClass] { get }
```

## Discussion

This property contains the value of transformedValueClass() if that value isn’t `nil`. Otherwise, it holds a list of the top level classes that it decodes, which includes NSArray, NSDictionary, NSSet, NSString, NSNumber, NSDate, NSData, NSURL, NSUUID, and NSNull.

Override this property in subclasses to provide an expanded or different set of allowed transformation classes.

