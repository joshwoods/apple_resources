

- AVKit
- AVExperienceController
- AVExperienceController.ExpandedConfiguration
-  AVExperienceController.ExpandedConfiguration.Placement 

Structure

# AVExperienceController.ExpandedConfiguration.Placement

A structure that represents where the video will be experienced.

visionOS 2.0+

``` source
struct Placement
```

## Overview

Control where an experience is placed. It can be over a UIScene.

## Topics

### Placements

static func over(scene: UIScene) -> AVExperienceController.ExpandedConfiguration.Placement

Places the video over the provided scene.

static var unspecified: AVExperienceController.ExpandedConfiguration.Placement

Doesn’t specify placement.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Specifying placement

var fallbackPlacement: AVExperienceController.ExpandedConfiguration.Placement

A fallback placement to use when the original container isn’t in the view controller hierarchy.

