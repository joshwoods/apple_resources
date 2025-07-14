

- PHASE
- PHASEGroup
-  isMuted 

Instance Property

# isMuted

A Boolean value that indicates whether the app silences the group.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var isMuted: Bool { get }
```

## See Also

### Silencing Sounds

func mute()

Silences the group.

func unmute()

Restores the group’s volume.

func solo()

Silences all other groups.

func unsolo()

Restores the other groups’ volume.

var isSoloed: Bool

A Boolean value that indicates whether the app silences all groups other than this group.

