

- Core Animation
- CATransaction
-  setAnimationDuration(\_:) 

Type Method

# setAnimationDuration(\_:)

Sets the animation duration used by all animations within this transaction group.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func setAnimationDuration(_ dur: CFTimeInterval)
```

## Parameters 

`dur`  

An interval of time used as the duration.

## Discussion

You can also set the animation duration for a specific transaction object by calling the setValue(_:forKey:) method of that object and specifying the kCATransactionAnimationDuration key.

## See Also

### Overriding Animation Duration and Timing

class func animationDuration() -> CFTimeInterval

Returns the animation duration used by all animations within this transaction group.

class func animationTimingFunction() -> CAMediaTimingFunction?

Returns the timing function used for all animations within this transaction group.

class func setAnimationTimingFunction(CAMediaTimingFunction?)

Sets the timing function used for all animations within this transaction group.

