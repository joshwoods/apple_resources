

- AVFoundation
- AVCaptureSlider
-  setActionQueue(\_:action:) 

Instance Method

# setActionQueue(\_:action:)

Sets the action to perform on the specified dispatch queue when the control’s value changes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
@nonobjc
func setActionQueue(
    _ actionQueue: DispatchQueue,
    action: @escaping (Float) -> ()
)
```

## Parameters 

`actionQueue`  

A dispatch queue on which to call the action.

`action`  

The action to perform in response to changes to the slider’s value.

## Mentioned in 

Enhancing your app experience with the Camera Control

## Discussion

If the action modifies a property of the camera system, the specified dispatch queue must represent the camera system’s same exclusive execution context (see isSameExclusiveExecutionContext(other:)).

