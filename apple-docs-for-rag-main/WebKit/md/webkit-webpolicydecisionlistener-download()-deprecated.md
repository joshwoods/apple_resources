

- WebKit
- WebPolicyDecisionListener
-  download() Deprecated

Instance Method

# download()

Tells the listener to download the resource instead of displaying it.

macOS 10.3–10.14Deprecated

``` source
func download()
```

**Required**

## Discussion

This method converts a location change that may be in progress to a download operation without having to stop and restart the download. You might invoke this method based on the content’s MIME type.

## See Also

### Making Resource-Usage Decisions

func ignore()

Tells the listener to ignore the resource.

**Required**

Deprecated

func use()

Tells the listener to use the resource.

**Required**

Deprecated

