

- CoreAudioKit
- AUGenericView
-  init(audioUnit:displayFlags:) 

Initializer

# init(audioUnit:displayFlags:)

Initializes a generic view for an audio unit, setting specific display flags.

macOS 10.4+

``` source
@MainActor
init(
    audioUnit inAudioUnit: AudioUnit,
    displayFlags inFlags: AUGenericViewDisplayFlags
)
```

## Parameters 

`inAudioUnit`  

The audio unit associated with the generic view.

`inFlags`  

One or more flags that specify display properties. You can combine multiple flags using the logical `OR` (`|`) operator. For the available flags, see `Generic View Display Flags`.

## Return Value

The initialized audio unit associated with the generic view, with display flags set.

## Topics

### Display Flags

struct AUGenericViewDisplayFlags

Flags that describe the display of a generic view.

## See Also

### Creating a Generic View

init(audioUnit: AudioUnit)

Creates a generic view for an audio unit, setting all display flags.

