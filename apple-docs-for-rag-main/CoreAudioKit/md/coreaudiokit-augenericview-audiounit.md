

- CoreAudioKit
- AUGenericView
-  audioUnit 

Instance Property

# audioUnit

The audio unit associated with the generic view.

macOS 10.4+

``` source
@MainActor
var audioUnit: AudioUnit { get }
```

## Discussion

The audio unit associated with the generic view. On error, returns `nil`.

