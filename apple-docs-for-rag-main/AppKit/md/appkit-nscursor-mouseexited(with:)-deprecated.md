

- AppKit
- NSCursor
-  mouseExited(with:) Deprecated

Instance Method

# mouseExited(with:)

Automatically sent to the receiver when the cursor exits a cursor rectangle owned by the receiver.

macOS 10.0–10.13Deprecated

``` source
func mouseExited(with event: NSEvent)
```

Deprecated

This method is not used.

## Parameters 

`event`  

The event generated when the cursor exits the cursor rectangle.

## Discussion

Like mouseEntered(with:), this message is part of the class interface only so you can override it.

For a more complete explanation, see Mouse-Tracking and Cursor-Update Events and the NSView method addTrackingRect(_:owner:userData:assumeInside:).

## See Also

### Controlling Which Cursor Is Current

class func pop()

Pops the current cursor off the top of the stack.

func pop()

Sends a pop() message to the receiver’s class.

func push()

Puts the receiver on top of the cursor stack and makes it the current cursor.

func set()

Makes the receiver the current cursor.

func mouseEntered(with: NSEvent)

Automatically sent to the receiver when the cursor enters a cursor rectangle owned by the receiver.

Deprecated

func setOnMouseEntered(Bool)

Specifies whether the receiver accepts mouseEntered(with:) events.

Deprecated

var isSetOnMouseEntered: Bool

A Boolean value indicating whether the receiver becomes current on receiving a mouseEntered(with:) message.

Deprecated

func setOnMouseExited(Bool)

Sets whether the receiver accepts mouseExited(with:) events.

Deprecated

var isSetOnMouseExited: Bool

A Boolean value indicating whether the receiver becomes current when it receives a mouseExited(with:) message.

Deprecated

