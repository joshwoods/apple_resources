

- Core ML
- MLPredictionOptions
-  usesCPUOnly Deprecated

Instance Property

# usesCPUOnly

A Boolean value that indicates whether a prediction is computed using only the CPU.

iOS 11.0–15.0DeprecatediPadOS 11.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.13–12.0DeprecatedtvOS 11.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 4.0–8.0Deprecated

``` source
var usesCPUOnly: Bool { get set }
```

## Discussion

Your model should be restricted to the CPU if it might run in the background or if your app has other GPU intensive tasks.

