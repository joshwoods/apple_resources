

- WebKit
- WKURLSchemeTask
-  didReceive(\_:) 

Instance Method

# didReceive(\_:)

Sends some or all of the resource data to WebKit.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func didReceive(_ data: Data)
```

**Required**

## Parameters 

`data`  

Data for the resource. This object may contain all of the data or only some of it.

## Discussion

Call this method to deliver any resource data back to WebKit. If you load the data incrementally, you may call this method multiple times to deliver each new portion of the data. Each time you call this method, WebKit appends the new data to any previously received data.

This method raises an exception if you call it before the didReceive(_:) method, or after the didFinish() method. It also raises an exception if you call it after WebKit calls the webView(_:stop:) method of the corresponding handler object.

## See Also

### Reporting Progress Back to WebKit

func didReceive(URLResponse)

Returns a URL response to WebKit with information about the requested resource.

**Required**

func didFinish()

Signals the successful completion of the task.

**Required**

