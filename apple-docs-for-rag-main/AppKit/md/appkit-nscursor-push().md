

- AppKit
- NSCursor
-  push() 

Instance Method

# push()

Puts the receiver on top of the cursor stack and makes it the current cursor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

``` source
func push()
```

## See Also

### Controlling Which Cursor Is Current

class func pop()

Pops the current cursor off the top of the stack.

func pop()

Sends a pop() message to the receiver’s class.

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

func mouseExited(with: NSEvent)

Automatically sent to the receiver when the cursor exits a cursor rectangle owned by the receiver.

Deprecated

func setOnMouseExited(Bool)

Sets whether the receiver accepts mouseExited(with:) events.

Deprecated

var isSetOnMouseExited: Bool

A Boolean value indicating whether the receiver becomes current when it receives a mouseExited(with:) message.

Deprecated

