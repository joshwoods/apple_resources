

- Quartz
- QCPlugInViewController
-  init(plugIn:viewNibName:) Deprecated

Initializer

# init(plugIn:viewNibName:)

Creates and initializes a controller for the specified `QCPlugIn` object and nib file.

macOS 10.4–10.15Deprecated

``` source
@MainActor
init!(
    plugIn: QCPlugIn!,
    viewNibName name: String!
)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`plugIn`  

A `QCPlugIn` object that uses internal settings.

`name`  

The name of the nib file that contains the view for the custom patch.

## Return Value

A `QCPlugInViewController` object.

