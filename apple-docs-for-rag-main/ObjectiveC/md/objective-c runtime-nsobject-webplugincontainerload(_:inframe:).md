

- Objective-C Runtime
- NSObject
-  webPlugInContainerLoad(\_:inFrame:) 

Instance Method

# webPlugInContainerLoad(\_:inFrame:)

Loads a URL into a web frame.

macOS

``` source
func webPlugInContainerLoad(
    _ request: URLRequest!,
    inFrame target: String!
)
```

## Parameters 

`request`  

The request that specifies the URL.

`target`  

The frame into which the URL is loaded.

## Discussion

If the frame specified by `target` is not found, a new window is opened, loaded with the URL request, and given the specified frame name. If `target` is `nil`, the frame enclosing the plug-in is loaded with the URL request.

## See Also

### Performing actions on the enclosing container

func webPlugInContainerShowStatus(String!)

Tells the container to show a status message.

