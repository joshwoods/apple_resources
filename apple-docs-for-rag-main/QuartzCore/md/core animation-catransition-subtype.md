

- Core Animation
- CATransition
-  subtype 

Instance Property

# subtype

Specifies an optional subtype that indicates the direction for the predefined motion-based transitions.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var subtype: CATransitionSubtype? { get set }
```

## Discussion

The possible values are shown in Common Transition Subtypes. The default is `nil`.

This property is ignored if a custom transition is specified in the filter property.

## See Also

### Transition Properties

var type: CATransitionType

Specifies the predefined transition type.

