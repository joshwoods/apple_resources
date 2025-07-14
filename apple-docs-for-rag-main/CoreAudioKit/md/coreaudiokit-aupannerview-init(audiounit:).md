

- CoreAudioKit
- AUPannerView
-  init(audioUnit:) 

Initializer

# init(audioUnit:)

Creates a panner view for an audio unit.

macOS 10.5+

``` source
@MainActor
init(audioUnit au: AudioUnit)
```

## Parameters 

`au`  

The panner audio unit associated with the panner view.

## Return Value

The newly instantiated panner view. On error, returns `nil`.

## Discussion

Call this static constructor as follows:

```
```

