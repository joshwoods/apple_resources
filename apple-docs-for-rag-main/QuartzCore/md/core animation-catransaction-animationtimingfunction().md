

- Core Animation
- CATransaction
-  animationTimingFunction() 

Type Method

# animationTimingFunction()

Returns the timing function used for all animations within this transaction group.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func animationTimingFunction() -> CAMediaTimingFunction?
```

## Return Value

An instance of `CAMediaTimingFunction`.

## Discussion

This is a convenience method that returns the CAMediaTimingFunction for the value(forKey:) value returned by the kCATransactionAnimationTimingFunction key.

## See Also

### Overriding Animation Duration and Timing

class func animationDuration() -> CFTimeInterval

Returns the animation duration used by all animations within this transaction group.

class func setAnimationDuration(CFTimeInterval)

Sets the animation duration used by all animations within this transaction group.

class func setAnimationTimingFunction(CAMediaTimingFunction?)

Sets the timing function used for all animations within this transaction group.

