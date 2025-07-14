

- WebKit
- WKURLSchemeTask
-  didFailWithError(\_:) 

Instance Method

# didFailWithError(\_:)

Completes the task and reports the specified error back to WebKit.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func didFailWithError(_ error: any Error)
```

**Required**

## Parameters 

`error`  

The error that caused the task to fail.

## Discussion

This method signals to WebKit that the task is complete, but failed with the specified error. Use this method to report any errors during the load process.

After calling this method, it’s a programmer error to call other methods of the task object, and those methods raise an exception if you do. This method raises an exception if you call it after WebKit calls the webView(_:stop:) method of the corresponding handler object.

