

- Cinematic
- CNScript
-  removeDetectionTrack(\_:) 

Instance Method

# removeDetectionTrack(\_:)

Removes the user-created detection track.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
final func removeDetectionTrack(_ detectionTrack: CNDetectionTrack) -> Bool
```

## Parameters 

`detectionTrack`  

The detection track to remove.

## Return Value

A flag indicating whether removal of the user-created detection track was successful.

## Discussion

It’s not possible to remove tracks created at recording time.

