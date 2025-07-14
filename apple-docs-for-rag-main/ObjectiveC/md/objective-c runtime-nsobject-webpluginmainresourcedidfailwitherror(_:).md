

- Objective-C Runtime
- NSObject
-  webPlugInMainResourceDidFailWithError(\_:) 

Instance Method

# webPlugInMainResourceDidFailWithError(\_:)

Invoked when an error occurs loading the main resource.

macOS 10.6+

``` source
func webPlugInMainResourceDidFailWithError(_ error: (any Error)!)
```

## Parameters 

`error`  

An error object containing details of why the connection failed to load the request successfully.

## Discussion

This message is invoked when the underlying `NSURLConnection` object for the main resource sends the connection:didFailWithError: message to its delegate.

## See Also

### Main resource messages

func webPlugInMainResourceDidFinishLoading()

Invoked when the connection successfully finishes loading data.

func webPlugInMainResourceDidReceive(Data!)

Invoked when the connection loads data incrementally.

func webPlugInMainResourceDidReceive(URLResponse!)

Invoked when the connection receives sufficient data to construct the URL response for its request.

