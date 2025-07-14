

- PHASE
- PHASEGroup
-  solo() 

Instance Method

# solo()

Silences all other groups.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func solo()
```

## Discussion

The engine silences all groups other than the group on which the app calls this function.

## See Also

### Silencing Sounds

func mute()

Silences the group.

func unmute()

Restores the group’s volume.

var isMuted: Bool

A Boolean value that indicates whether the app silences the group.

func unsolo()

Restores the other groups’ volume.

var isSoloed: Bool

A Boolean value that indicates whether the app silences all groups other than this group.

