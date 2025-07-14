

- Matter
- MTRServerAttribute
-  newFeatureMapAttribute(withInitialValue:) 

Type Method

# newFeatureMapAttribute(withInitialValue:)

Create an attribute description for a FeatureMap attribute with the provided value (expected to be an unsigned integer representing the value of the bitmap). This will automatically set requiredPrivilege to the right value for FeatureMap.

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class func newFeatureMapAttribute(withInitialValue value: NSNumber) -> Self
```

