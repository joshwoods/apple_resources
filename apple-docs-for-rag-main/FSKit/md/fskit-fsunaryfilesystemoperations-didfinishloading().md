

- FSKit
- FSUnaryFileSystemOperations
-  didFinishLoading() 

Instance Method

# didFinishLoading()

Notifies you that the system finished loading your file system extension.

macOS 15.4+

``` source
optional func didFinishLoading()
```

## Discussion

The system performs this callback after the main run loop starts and before receiving the first message from the FSKit daemon.

Implement this method if you want to perform any setup prior to receiving FSKit callbacks.

## See Also

### Loading and unloading resources

func loadResource(resource: FSResource, options: FSTaskOptions, replyHandler: (FSVolume?, (any Error)?) -> Void)

Requests that the file system load a resource and present it as a volume.

**Required**

func unloadResource(resource: FSResource, options: FSTaskOptions, replyHandler: ((any Error)?) -> Void)

Requests that the file system unload the specified resource.

**Required**

