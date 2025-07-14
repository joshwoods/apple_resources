

- Objective-C Runtime
- NSObject
-  compositionPickerViewDidStartAnimating(\_:) Deprecated

Instance Method

# compositionPickerViewDidStartAnimating(\_:)

Performs custom tasks when the composition picker view starts animating a composition.

macOS 10.4–10.15Deprecated

``` source
func compositionPickerViewDidStartAnimating(_ pickerView: QCCompositionPickerView!)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`pickerView`  

The composition picker view in which the composition started animating.

## Discussion

Quartz Composer invokes this method when the composition picker view starts animating a composition. Implement this method if you want to perform custom tasks at that time.

