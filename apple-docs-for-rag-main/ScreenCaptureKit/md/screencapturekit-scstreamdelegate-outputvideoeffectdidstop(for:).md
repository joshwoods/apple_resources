

- ScreenCaptureKit
- SCStreamDelegate
-  outputVideoEffectDidStop(for:) 

Instance Method

# outputVideoEffectDidStop(for:)

Tells the delegate that Presenter Overlay stopped.

Mac Catalyst 17.0+macOS 14.0+

``` source
optional func outputVideoEffectDidStop(for stream: SCStream)
```

## Parameters 

`stream`  

The stream that was using Presenter Overlay.

## See Also

### Responding to Presenter Overlay

func outputVideoEffectDidStart(for: SCStream)

Tells the delegate that Presenter Overlay started.

