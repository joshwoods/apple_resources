

- WebKit
- DOMMouseEvent
-  initMouseEvent(\_:canBubble:cancelable:view:detail:screenX:screenY:clientX:clientY:ctrlKey:altKey:shiftKey:metaKey:button:relatedTarget:) Deprecated

Instance Method

# initMouseEvent(\_:canBubble:cancelable:view:detail:screenX:screenY:clientX:clientY:ctrlKey:altKey:shiftKey:metaKey:button:relatedTarget:)

macOS 10.5–10.14Deprecated

``` source
func initMouseEvent(
    _ type: String!,
    canBubble: Bool,
    cancelable: Bool,
    view: DOMAbstractView!,
    detail: Int32,
    screenX: Int32,
    screenY: Int32,
    clientX: Int32,
    clientY: Int32,
    ctrlKey: Bool,
    altKey: Bool,
    shiftKey: Bool,
    metaKey: Bool,
    button: UInt16,
    relatedTarget: (any DOMEventTarget)!
)
```

