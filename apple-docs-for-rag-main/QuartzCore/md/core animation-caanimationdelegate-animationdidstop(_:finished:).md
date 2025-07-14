

- Core Animation
- CAAnimationDelegate
-  animationDidStop(\_:finished:) 

Instance Method

# animationDidStop(\_:finished:)

Tells the delegate the animation has ended.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
optional func animationDidStop(
    _ anim: CAAnimation,
    finished flag: Bool
)
```

## Parameters 

`anim`  

The CAAnimation object that has ended.

`flag`  

A flag indicating whether the animation has completed by reaching the end of its duration.

## Discussion

The animation may have ended because it has completed its active duration or because it has been removed from the layer it is attached to. `flag` is true if the animation reached the end of its duration without being removed.

## See Also

### Customizing Start and Stop Times

func animationDidStart(CAAnimation)

Tells the delegate the animation has started.

