

- AppKit
- NSScrollView
-  tile() 

Instance Method

# tile()

Lays out the components of the receiver: the content view, the scrollers, and the ruler views.

macOS

``` source
@MainActor
func tile()
```

## Discussion

You rarely need to invoke this method, but subclasses may override it to manage additional components.

