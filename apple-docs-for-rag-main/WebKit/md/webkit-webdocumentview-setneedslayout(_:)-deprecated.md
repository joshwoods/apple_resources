

- WebKit
- WebDocumentView
-  setNeedsLayout(\_:) Deprecated

Instance Method

# setNeedsLayout(\_:)

Sets whether or not the receiver should change its layout.

macOS 10.3–10.14Deprecated

``` source
func setNeedsLayout(_ flag: Bool)
```

**Required**

## Parameters 

`flag`  

Sets whether the receiver needs to update its layout in the next call to its draw(_:) method.

## Discussion

A view conforming to this protocol should store the most recent value of this flag in an internal variable. Then, in its drawRect method, if the most recent value of this flag was true, it should invoke layout() and reset the internal variable before updating the contents of the view.

## See Also

### Controlling the layout

func layout()

Invoked when the receiver should change its layout immediately.

**Required**

Deprecated

