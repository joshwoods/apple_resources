

- PHASE
- PHASEEngine
- PHASEEngine.UpdateMode
-  PHASEEngine.UpdateMode.manual 

Case

# PHASEEngine.UpdateMode.manual

A mode that indicates the app controls when the framework adjusts state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case manual
```

## Discussion

In this mode, the framework waits for the app to call update() before processing the app’s API calls and adjusting internal states.

## See Also

### Modes

case automatic

A mode that indicates PHASE sets the timing of state adjustments.

