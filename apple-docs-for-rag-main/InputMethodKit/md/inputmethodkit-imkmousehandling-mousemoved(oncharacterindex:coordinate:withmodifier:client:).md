

- InputMethodKit
- IMKMouseHandling
-  mouseMoved(onCharacterIndex:coordinate:withModifier:client:) 

Instance Method

# mouseMoved(onCharacterIndex:coordinate:withModifier:client:)

Handles a mouse-moved event sent to an input method.

macOS 10.5+

``` source
func mouseMoved(
    onCharacterIndex index: Int,
    coordinate point: NSPoint,
    withModifier flags: Int,
    client sender: Any!
) -> Bool
```

**Required**

## Parameters 

`index`  

The index within the sender’s text storage where the mouse-moved event occurred.

`point`  

The point at which the mouse-moved event occurred.

`flags`  

The modifier keys.

`sender`  

The client object.

## Return Value

true if handled; otherwise false.

## Discussion

Implement this method if your input method handles mouse-moved events.

## See Also

### Handling Mouse Events

func mouseDown(onCharacterIndex: Int, coordinate: NSPoint, withModifier: Int, continueTracking: UnsafeMutablePointer&lt;ObjCBool>!, client: Any!) -> Bool

Handles mouse-down event send to an input method.

**Required**

func mouseUp(onCharacterIndex: Int, coordinate: NSPoint, withModifier: Int, client: Any!) -> Bool

Handles a mouse-up event sent to an input method.

**Required**

