

- SceneKit
- SCNView
-  pause(\_:) 

Instance Method

# pause(\_:)

Pauses playback of the view’s scene.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@IBAction @MainActor
func pause(_ sender: Any?)
```

## Parameters 

`sender`  

The object requesting the action (used when connecting a control in Interface Builder). SceneKit ignores this parameter.

## Discussion

This method has no effect if the scene is already paused.

## See Also

### Playing Action and Animation in a View’s Scene

func play(Any?)

Resumes playback of the view’s scene.

func stop(Any?)

Stops playback of the view’s scene and resets the scene time to its start time.

