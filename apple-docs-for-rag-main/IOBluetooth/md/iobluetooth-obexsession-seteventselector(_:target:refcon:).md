

- IOBluetooth
- OBEXSession
-  setEventSelector(\_:target:refCon:) 

Instance Method

# setEventSelector(\_:target:refCon:)

Allow you to set a selector to be called when events occur on the OBEX session.

macOS

``` source
func setEventSelector(
    _ inEventSelector: Selector!,
    target inEventSelectorTarget: Any!,
    refCon inUserRefCon: UnsafeMutableRawPointer!
)
```

## Parameters 

`inEventSelector`  

Selector to call on the target.

`inEventSelectorTarget`  

Target to be called with the selector.

`inUserRefCon`  

User’s refCon that will get passed when their event callback is invoked.

## Discussion

Really not needed to be used, since the event selector will get set when an OBEX command is sent out.

