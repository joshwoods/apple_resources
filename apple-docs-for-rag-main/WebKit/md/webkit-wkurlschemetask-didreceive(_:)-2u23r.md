

- WebKit
- WKURLSchemeTask
-  didReceive(\_:) 

Instance Method

# didReceive(\_:)

Returns a URL response to WebKit with information about the requested resource.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func didReceive(_ response: URLResponse)
```

**Required**

## Parameters 

`response`  

The response to return to WebKit. Your response object must include the MIME type of the requested resource.

## Discussion

Call this method to provide WebKit with the MIME type of the requested resource and its expected size. You must call this method at least once for each task, and you may call it multiple times if needed. Always call it before sending any data back to WebKit using the didReceive(_:) method.

It is a programmer error to call this method after calling the didFinish() method of the same task object. It is also a programmer error to call this method after WebKit calls the webView(_:stop:) method of the corresponding handler object. If you do, this method raises an exception in both cases.

## See Also

### Reporting Progress Back to WebKit

func didReceive(Data)

Sends some or all of the resource data to WebKit.

**Required**

func didFinish()

Signals the successful completion of the task.

**Required**

