

- WebKit
- WebDocumentView
-  layout() Deprecated

Instance Method

# layout()

Invoked when the receiver should change its layout immediately.

macOS 10.3–10.14Deprecated

``` source
func layout()
```

**Required**

## Discussion

This message is sent to the view as a hint to perform any calculations and update rendering information. For example, at a minimum, the receiver might set the frame rectangle. This method should not perform any drawing operations.

## See Also

### Controlling the layout

func setNeedsLayout(Bool)

Sets whether or not the receiver should change its layout.

**Required**

Deprecated

