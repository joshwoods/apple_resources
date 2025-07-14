

- Metal
- MTLResourceOptions
-  hazardTrackingModeTracked 

Type Property

# hazardTrackingModeTracked

An option specifying that Metal prevents hazards when modifying this object’s contents.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
static var hazardTrackingModeTracked: MTLResourceOptions { get }
```

## Discussion

For more information, see MTLHazardTrackingMode.tracked.

## See Also

### Specifying Hazard Tracking

static var hazardTrackingModeUntracked: MTLResourceOptions

An option specifying that the app must prevent hazards when modifying this object’s contents.

