

- PHASE
- PHASEEngine
-  activeGroupPreset 

Instance Property

# activeGroupPreset

The settings that define playback for a group of sounds.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var activeGroupPreset: PHASEGroupPreset? { get }
```

## Discussion

This property returns the most recent group preset on which the app calls activate(). Group presets map a collection of sounds in a group to settings the app applies in a specific context. For more information, see PHASEGroupPreset.

## See Also

### Managing Groups of Sounds

var groups: [String : PHASEGroup]

A list of named groups that contain sounds the app operates on collectively.

var duckers: [PHASEDucker]

An array of objects that reduce the volume of simultaneously playing sounds.

