

- Core Animation
- CATransition
-  type 

Instance Property

# type

Specifies the predefined transition type.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var type: CATransitionType { get set }
```

## Discussion

The possible values are shown in Common Transition Types. This property is ignored if a custom transition is specified in the filter property. The default is fade.

## See Also

### Transition Properties

var subtype: CATransitionSubtype?

Specifies an optional subtype that indicates the direction for the predefined motion-based transitions.

