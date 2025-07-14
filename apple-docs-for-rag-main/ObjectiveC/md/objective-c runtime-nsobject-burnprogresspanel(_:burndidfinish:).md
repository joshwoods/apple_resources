

- Objective-C Runtime
- NSObject
-  burnProgressPanel(\_:burnDidFinish:) 

Instance Method

# burnProgressPanel(\_:burnDidFinish:)

Allows the delegate to handle the end-of-burn feedback.

macOS

``` source
func burnProgressPanel(
    _ theBurnPanel: DRBurnProgressPanel!,
    burnDidFinish burn: DRBurn!
) -> Bool
```

## Parameters 

`theBurnPanel`  

The progress panel

`burn`  

The object that performed the burn.

## Return Value

A `BOOL` indicating whether the normal end-of-burn feedback should occur.

## Discussion

This method allows the delegate to handle or modify the end-of-burn feedback performed by the progress panel. Return `YES` to indicate the delegate handled the burn completion and the standard feedback should be supressed. If this method returns `NO`, the normal end-of-burn handling is performed (displaying an error if appropriate, playing an “I’m done” sound, etc).

The delegate is messaged before the progress panel is ordered out so a sheet may be displayed on a progress panel displayed as a window.

