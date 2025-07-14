

- Quick Look UI
- QLPreviewView
-  shouldCloseWithWindow 

Instance Property

# shouldCloseWithWindow

A Boolean value that determines whether the preview should close when its window closes.

macOS 10.6+

``` source
@MainActor
var shouldCloseWithWindow: Bool { get set }
```

## Discussion

The default value of this property is true, which means that the preview automatically closes when its window closes. If you set this property to false, close the preview by calling the close() method when finished with it. Once you close a QLPreviewView, it won’t accept any more preview items.

## See Also

### Closing a Preview

func close()

Closes the view, releasing the current preview item.

