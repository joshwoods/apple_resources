

- AVKit
- AVExperienceController
- AVExperienceController.Experience
-  AVExperienceController.Experience.embedded 

Case

# AVExperienceController.Experience.embedded

An experience where the video embeds within its original container.

visionOS 2.0+

``` source
case embedded
```

## Discussion

This experience is the starting state and is valid on all platforms. You may embed video in the original container even if that container isn’t visible or not in the view hierarchy. It’s valid to transition to this experience from any other experience, even when the player view controller isn’t in the view hierarchy.

It’s the app’s responsibility to correctly manage the player view controller’s view lifecycle.

Note

This experience to is analogous to a player view controller’s inline state.

## See Also

### Supported experiences

case expanded

An experience where the system places the video outside of its original container.

case multiview

An experience where multiple videos play together.

