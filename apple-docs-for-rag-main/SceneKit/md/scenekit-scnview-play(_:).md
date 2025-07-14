

- SceneKit
- SCNView
-  play(\_:) 

Instance Method

# play(\_:)

Resumes playback of the view’s scene.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@IBAction @MainActor
func play(_ sender: Any?)
```

## Parameters 

`sender`  

The object requesting the action (used when connecting a control in Interface Builder). SceneKit ignores this parameter.

## Discussion

This method has no effect if the scene is not paused.

## See Also

### Playing Action and Animation in a View’s Scene

func pause(Any?)

Pauses playback of the view’s scene.

func stop(Any?)

Stops playback of the view’s scene and resets the scene time to its start time.

