

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
-  startSubmission() 

Instance Method

# startSubmission()

Notifies Compositor Services that you’re ready to generate the Metal commands to render the specified frame.

visionOS 1.0+

``` source
func startSubmission()
```

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

This function helps you optimize your app’s rendering efficiency. Call it before you start any of the GPU work that depends on the device pose. Call endSubmission() after you build your Metal command buffers and are ready to commit the frame to the GPU. Compositor Services uses the time difference to improve its predictions for when to start the frame submission process. Those predictions help you schedule the encoding process at a more optimal time for the system.

## See Also

### Reporting frame submission times

func endSubmission()

Notifies Compositor Services that you finished generating the GPU commands to render the specified frame.

