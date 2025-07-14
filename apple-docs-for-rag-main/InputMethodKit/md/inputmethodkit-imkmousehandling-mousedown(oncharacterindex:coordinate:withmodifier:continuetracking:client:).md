

- InputMethodKit
- IMKMouseHandling
-  mouseDown(onCharacterIndex:coordinate:withModifier:continueTracking:client:) 

Instance Method

# mouseDown(onCharacterIndex:coordinate:withModifier:continueTracking:client:)

Handles mouse-down event send to an input method.

macOS 10.0+

``` source
func mouseDown(
    onCharacterIndex index: Int,
    coordinate point: NSPoint,
    withModifier flags: Int,
    continueTracking keepTracking: UnsafeMutablePointer!,
    client sender: Any!
) -> Bool
```

**Required**

## Parameters 

`index`  

The index within the sender’s text storage where the mouse-down event occurred.

`point`  

The point at which the mouse-down event occurred.

`flags`  

The modifier keys.

`keepTracking`  

Set this parameter to true if you want to receive subsequent mouse-moved and mouse -up events.

`sender`  

The client object.

## Return Value

true if handled; otherwise false.

## Discussion

Implement this method if your input method handles mouse-down events.

## See Also

### Handling Mouse Events

func mouseUp(onCharacterIndex: Int, coordinate: NSPoint, withModifier: Int, client: Any!) -> Bool

Handles a mouse-up event sent to an input method.

**Required**

func mouseMoved(onCharacterIndex: Int, coordinate: NSPoint, withModifier: Int, client: Any!) -> Bool

Handles a mouse-moved event sent to an input method.

**Required**

