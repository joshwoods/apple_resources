

- AppKit
- NSCursor
-  setOnMouseEntered(\_:) Deprecated

Instance Method

# setOnMouseEntered(\_:)

Specifies whether the receiver accepts mouseEntered(with:) events.

macOS 10.0–10.13Deprecated

``` source
func setOnMouseEntered(_ flag: Bool)
```

Deprecated

This method is not used.

## Parameters 

`flag`  

true if the receiver accepts future mouseEntered(with:) event messages; otherwise it ignores them.

## Discussion

Accepting mouseEntered(with:) event messages allows the cursor to be made the current cursor when the cursor enters a view’s cursor rectangle.

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

var isSetOnMouseEntered: Bool

A Boolean value indicating whether the receiver becomes current on receiving a mouseEntered(with:) message.

Deprecated

func mouseExited(with: NSEvent)

Automatically sent to the receiver when the cursor exits a cursor rectangle owned by the receiver.

Deprecated

func setOnMouseExited(Bool)

Sets whether the receiver accepts mouseExited(with:) events.

Deprecated

var isSetOnMouseExited: Bool

A Boolean value indicating whether the receiver becomes current when it receives a mouseExited(with:) message.

Deprecated

