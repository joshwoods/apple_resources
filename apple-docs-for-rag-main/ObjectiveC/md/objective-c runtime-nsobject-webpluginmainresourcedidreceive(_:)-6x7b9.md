

- Objective-C Runtime
- NSObject
-  webPlugInMainResourceDidReceive(\_:) 

Instance Method

# webPlugInMainResourceDidReceive(\_:)

Invoked when the connection receives sufficient data to construct the URL response for its request.

macOS 10.6+

``` source
func webPlugInMainResourceDidReceive(_ response: URLResponse!)
```

## Parameters 

`response`  

The URL response for the connection’s request.

## Discussion

This message is invoked when the `WebPlugInShouldLoadMainResourceKey` plug-in command-line argument is set to NO and the underlying `NSURLConnection` object for the main resource sends the connection:didReceiveResponse: message to its delegate.

## See Also

### Main resource messages

func webPlugInMainResourceDidFailWithError((any Error)!)

Invoked when an error occurs loading the main resource.

func webPlugInMainResourceDidFinishLoading()

Invoked when the connection successfully finishes loading data.

func webPlugInMainResourceDidReceive(Data!)

Invoked when the connection loads data incrementally.

