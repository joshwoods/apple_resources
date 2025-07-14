

- Objective-C Runtime
- NSObject
-  webPlugInMainResourceDidFinishLoading() 

Instance Method

# webPlugInMainResourceDidFinishLoading()

Invoked when the connection successfully finishes loading data.

macOS 10.6+

``` source
func webPlugInMainResourceDidFinishLoading()
```

## Discussion

This message is invoked when the `WebPlugInShouldLoadMainResourceKey` plug-in command-line argument is set to NO and the underlying `NSURLConnection` object for the main resource sends the connectionDidFinishLoading: message to its delegate.

## See Also

### Main resource messages

func webPlugInMainResourceDidFailWithError((any Error)!)

Invoked when an error occurs loading the main resource.

func webPlugInMainResourceDidReceive(Data!)

Invoked when the connection loads data incrementally.

func webPlugInMainResourceDidReceive(URLResponse!)

Invoked when the connection receives sufficient data to construct the URL response for its request.

