

- Objective-C Runtime
- NSObject
-  compositionPickerView(\_:didSelect:) Deprecated

Instance Method

# compositionPickerView(\_:didSelect:)

Performs custom tasks when the selected composition in the composition picker view changes.

macOS 10.4–10.15Deprecated

``` source
func compositionPickerView(
    _ pickerView: QCCompositionPickerView!,
    didSelect composition: QCComposition!
)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`pickerView`  

The composition picker view in which the selection changed.

`composition`  

The selected composition or `nil` if the previously selected composition is no longer selected.

## Discussion

Quartz Composer invokes this method when the selected composition in the composition picker view changes. Implement this method if you want to perform custom tasks at that time.

