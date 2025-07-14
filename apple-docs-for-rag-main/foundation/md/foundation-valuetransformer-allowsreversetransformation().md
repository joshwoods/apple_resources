

- Foundation
- ValueTransformer
-  allowsReverseTransformation() 

Type Method

# allowsReverseTransformation()

Returns a Boolean value that indicates whether the receiver can reverse a transformation.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func allowsReverseTransformation() -> Bool
```

## Return Value

true if the receiver supports reverse value transformations, otherwise false.

The default is true.

## Discussion

Subclasses should override this method to return false if they do not support reverse value transformations.

## See Also

### Getting Information About a Transformer

class func transformedValueClass() -> AnyClass

Returns the class of the value returned by the receiver for a forward transformation.

