

- Quick Look UI
- QLPreviewView
-  close() 

Instance Method

# close()

Closes the view, releasing the current preview item.

macOS 10.6+

``` source
@MainActor
func close()
```

## Discussion

Once a QLPreviewView is closed, it won’t accept any more preview items. You only need to call this method if shouldCloseWithWindow is set to false. If you don’t close a QLPreviewView when you are done using it, your app will leak memory.

## See Also

### Closing a Preview

var shouldCloseWithWindow: Bool

A Boolean value that determines whether the preview should close when its window closes.

