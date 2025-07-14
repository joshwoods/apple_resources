

- Objective-C Runtime
- NSObject
-  accessibilityDropPointDescriptors 

Instance Property

# accessibilityDropPointDescriptors

An array of location descriptor objects that you use to define where drops are possible on this element.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var accessibilityDropPointDescriptors: [UIAccessibilityLocationDescriptor]? { get set }
```

## Discussion

To restore the default automatic behavior for this property, assign or return the default value of `nil`.

Note

A value of `nil` does not describe the same behavior as the empty array, which specifies that there are no relevant interactions for this element.

## See Also

### Fine-Tuning Drag and Drop

var accessibilityDragSourceDescriptors: [UIAccessibilityLocationDescriptor]?

An array of location descriptor objects that you use to define what drags are possible from this element.

