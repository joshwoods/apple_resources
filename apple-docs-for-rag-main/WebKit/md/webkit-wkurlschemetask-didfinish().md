

- WebKit
- WKURLSchemeTask
-  didFinish() 

Instance Method

# didFinish()

Signals the successful completion of the task.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func didFinish()
```

**Required**

## Discussion

This method signals to WebKit that it has all of the resource’s data and the task is now complete. Call this method after sending a response and the resource data to WebKit using the didReceive(_:) and didReceive(_:) methods.

This method raises an exception if you call it before the didReceive(_:) method, or if the task is already complete. It also raises an exception if you call it after WebKit calls the webView(_:stop:) method of the corresponding handler object.

## See Also

### Reporting Progress Back to WebKit

func didReceive(URLResponse)

Returns a URL response to WebKit with information about the requested resource.

**Required**

func didReceive(Data)

Sends some or all of the resource data to WebKit.

**Required**

