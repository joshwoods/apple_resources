

- Foundation
- ValueTransformer
-  transformedValueClass() 

Type Method

# transformedValueClass()

Returns the class of the value returned by the receiver for a forward transformation.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func transformedValueClass() -> AnyClass
```

## Return Value

The class of the value returned by the receiver for a forward transformation.

## Discussion

A subclass should override this method to return the appropriate class.

## See Also

### Getting Information About a Transformer

class func allowsReverseTransformation() -> Bool

Returns a Boolean value that indicates whether the receiver can reverse a transformation.

