

- CoreAudioKit
- AUGenericView
-  init(audioUnit:) 

Initializer

# init(audioUnit:)

Creates a generic view for an audio unit, setting all display flags.

macOS 10.4+

``` source
@MainActor
init(audioUnit au: AudioUnit)
```

## Parameters 

`au`  

The audio unit associated with the generic view.

## Return Value

The initialized generic view. On error, returns `nil`.

## See Also

### Creating a Generic View

init(audioUnit: AudioUnit, displayFlags: AUGenericViewDisplayFlags)

Initializes a generic view for an audio unit, setting specific display flags.

