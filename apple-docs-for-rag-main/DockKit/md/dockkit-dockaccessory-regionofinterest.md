

- DockKit
- DockAccessory
-  regionOfInterest 

Instance Property

# regionOfInterest

The area in the video frame in which the dock accessory tracks a subject.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final var regionOfInterest: CGRect { get }
```

## See Also

### Performing animation

func animate(motion: DockAccessory.Animation) async throws -> Progress

Starts an animation sequence.

func setRegionOfInterest(CGRect) async throws

Sets the area in the video frame in which the dock accessory tracks a subject.

enum Animation

Character animations that describe how to move the dock accessory.

