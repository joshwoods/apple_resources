

- Objective-C Runtime
- NSObject
-  compositionPickerViewWillStopAnimating(\_:) Deprecated

Instance Method

# compositionPickerViewWillStopAnimating(\_:)

Performs custom tasks when the composition picker view stops animating a composition.

macOS 10.4–10.15Deprecated

``` source
func compositionPickerViewWillStopAnimating(_ pickerView: QCCompositionPickerView!)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`pickerView`  

The composition picker view in which the composition stopped animating.

## Discussion

Quartz Composer invokes this method whenever the composition picker view stops animating a composition. Implement this method if you want to perform custom tasks at that time.

