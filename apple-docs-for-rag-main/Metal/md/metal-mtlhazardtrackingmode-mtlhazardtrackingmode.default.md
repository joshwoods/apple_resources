

- Metal
- MTLHazardTrackingMode
-  MTLHazardTrackingMode.default 

Case

# MTLHazardTrackingMode.default

An option specifying that the default tracking mode should be used.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
case `default`
```

## Discussion

The default behavior varies depending on the type of object being tracked:

| Resource | MTLHazardTrackingMode.tracked |
|----|----|
| Heap | MTLHazardTrackingMode.untracked |

## See Also

### Specifying the Tracking Mode

case untracked

An option specifying that the app must prevent hazards when modifying this object’s contents.

case tracked

An option specifying that Metal prevents hazards when modifying this object’s contents.

