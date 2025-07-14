

- AppKit
- NSResponder
-  performKeyEquivalent(with:) 

Instance Method

# performKeyEquivalent(with:)

Handle a key equivalent.

macOS

``` source
@MainActor
func performKeyEquivalent(with event: NSEvent) -> Bool
```

## Parameters 

`event`  

An event object that represents the key equivalent pressed.

## Discussion

Override to handle key equivalents. If the character code or codes in `event` match the receiver’s key equivalent, the receiver should respond to the event and return true. The default implementation does nothing and returns false.

Note

performKeyEquivalent(with:) takes an NSEvent object as its argument, while performMnemonic: takes an NSString object containing the uninterpreted characters of the key event. You should extract the characters for a key equivalent using the `NSEvent` method charactersIgnoringModifiers.

## See Also

### Related Documentation

func performKeyEquivalent(with: NSEvent) -> Bool

Implemented by subclasses to respond to key equivalents (also known as keyboard shortcuts).

func performKeyEquivalent(with: NSEvent) -> Bool

Checks the button’s key equivalent against the specified event and, if they match, simulates the button being clicked.

### Responding to Key Events

func keyDown(with: NSEvent)

Informs the receiver that the user has pressed a key.

func keyUp(with: NSEvent)

Informs the receiver that the user has released a key.

func interpretKeyEvents([NSEvent])

Handles a series of key events.

func flushBufferedKeyEvents()

Clears any unprocessed key events when overridden by subclasses.

