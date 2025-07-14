

- ScreenCaptureKit
- SCStreamDelegate
-  outputVideoEffectDidStart(for:) 

Instance Method

# outputVideoEffectDidStart(for:)

Tells the delegate that Presenter Overlay started.

Mac Catalyst 17.0+macOS 14.0+

``` source
optional func outputVideoEffectDidStart(for stream: SCStream)
```

## Parameters 

`stream`  

The stream using Presenter Overlay.

## See Also

### Responding to Presenter Overlay

func outputVideoEffectDidStop(for: SCStream)

Tells the delegate that Presenter Overlay stopped.

