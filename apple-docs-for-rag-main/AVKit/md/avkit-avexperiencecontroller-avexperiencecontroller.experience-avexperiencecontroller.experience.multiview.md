

- AVKit
- AVExperienceController
- AVExperienceController.Experience
-  AVExperienceController.Experience.multiview 

Case

# AVExperienceController.Experience.multiview

An experience where multiple videos play together.

visionOS 2.0+

``` source
case multiview
```

## Discussion

Configure this experience type using an AVMultiviewManager.

It’s valid to transition to this experience from a player view controller that isn’t in a view hierarchy. This is useful when adding additional videos to a multiview experience.

Transition to embedded to remove an item from the multiview experience.

## See Also

### Supported experiences

case embedded

An experience where the video embeds within its original container.

case expanded

An experience where the system places the video outside of its original container.

