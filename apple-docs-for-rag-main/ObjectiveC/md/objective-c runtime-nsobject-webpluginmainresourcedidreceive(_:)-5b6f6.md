

- Objective-C Runtime
- NSObject
-  webPlugInMainResourceDidReceive(\_:) 

Instance Method

# webPlugInMainResourceDidReceive(\_:)

Invoked when the connection loads data incrementally.

macOS 10.6+

``` source
func webPlugInMainResourceDidReceive(_ data: Data!)
```

## Parameters 

`data`  

The newly available data.

## Discussion

This message is invoked when the `WebPlugInShouldLoadMainResourceKey` plug-in command-line argument is set to NO and the underlying `NSURLConnection` object for the main resource sends the connection:didReceiveData: message to its delegate.

## See Also

### Main resource messages

func webPlugInMainResourceDidFailWithError((any Error)!)

Invoked when an error occurs loading the main resource.

func webPlugInMainResourceDidFinishLoading()

Invoked when the connection successfully finishes loading data.

func webPlugInMainResourceDidReceive(URLResponse!)

Invoked when the connection receives sufficient data to construct the URL response for its request.

