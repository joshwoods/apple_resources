

- WebKit
- WebPolicyDecisionListener
-  ignore() Deprecated

Instance Method

# ignore()

Tells the listener to ignore the resource.

macOS 10.3–10.14Deprecated

``` source
func ignore()
```

**Required**

## Discussion

You might invoke this method to handle the resource request yourself. For example, you might want to open a new window, open a window behind the current window, open a URL in an external application, or show a file URL location in the Finder.

## See Also

### Making Resource-Usage Decisions

func download()

Tells the listener to download the resource instead of displaying it.

**Required**

Deprecated

func use()

Tells the listener to use the resource.

**Required**

Deprecated

