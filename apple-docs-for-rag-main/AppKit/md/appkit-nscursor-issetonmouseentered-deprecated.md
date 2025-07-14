

- AppKit
- NSCursor
-  isSetOnMouseEntered Deprecated

Instance Property

# isSetOnMouseEntered

A Boolean value indicating whether the receiver becomes current on receiving a mouseEntered(with:) message.

macOS 10.0–10.13Deprecated

``` source
var isSetOnMouseEntered: Bool { get }
```

Deprecated

This method is not used.

## Discussion

true if the receiver will become current when it receives a mouseEntered(with:) message; otherwise, false.

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

func mouseExited(with: NSEvent)

Automatically sent to the receiver when the cursor exits a cursor rectangle owned by the receiver.

Deprecated

func setOnMouseExited(Bool)

Sets whether the receiver accepts mouseExited(with:) events.

Deprecated

var isSetOnMouseExited: Bool

A Boolean value indicating whether the receiver becomes current when it receives a mouseExited(with:) message.

Deprecated

