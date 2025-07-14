

- Metal
- MTLHazardTrackingMode
-  MTLHazardTrackingMode.untracked 

Case

# MTLHazardTrackingMode.untracked

An option specifying that the app must prevent hazards when modifying this object’s contents.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
case untracked
```

## Discussion

Metal does not do any dependency analysis on untracked resources. You are responsible for ensuring that resources are modified safely. See Resource Synchronization. When you already have detailed knowledge of how your app works, using untracked resources can improve performance.

## See Also

### Specifying the Tracking Mode

case `default`

An option specifying that the default tracking mode should be used.

case tracked

An option specifying that Metal prevents hazards when modifying this object’s contents.

