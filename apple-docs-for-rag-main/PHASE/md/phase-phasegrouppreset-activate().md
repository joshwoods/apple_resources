

- PHASE
- PHASEGroupPreset
-  activate() 

Instance Method

# activate()

Applies settings to the designated groups.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func activate()
```

## Discussion

When you call this function, the framework assigns the group preset as the engine’s activeGroupPreset and deactivates the previous assignee, as needed. The settings take effect according to timeToTarget.

## See Also

### Activating a Group Preset

func activate(timeToTargetOverride: Double)

Applies settings with an overriden fade duration.

