

- PHASE
- PHASEGroupPreset
-  deactivate() 

Instance Method

# deactivate()

Reverts settings for the preset’s groups.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func deactivate()
```

## Discussion

When you call this function, the framework restores the group’s default state by removing the preset’s settings. The settings fade over the timeToReset duration, and the engine removes the preset from activeGroupPreset.

## See Also

### Deactivating a Group Preset

func deactivate(timeToResetOverride: Double)

Reverts settings for the preset’s groups using a timed adjustment.

