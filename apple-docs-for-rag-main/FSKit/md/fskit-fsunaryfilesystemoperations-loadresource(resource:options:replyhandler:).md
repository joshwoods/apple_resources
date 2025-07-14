

- FSKit
- FSUnaryFileSystemOperations
-  loadResource(resource:options:replyHandler:) 

Instance Method

# loadResource(resource:options:replyHandler:)

Requests that the file system load a resource and present it as a volume.

macOS 15.4+

``` source
func loadResource(
    resource: FSResource,
    options: FSTaskOptions,
    replyHandler: @escaping (FSVolume?, (any Error)?) -> Void
)
```

**Required**

## Parameters 

`resource`  

An FSResource to load.

`options`  

An FSTaskOptions object specifying options to apply when loading the resource. An FSUnaryFileSystem supports two options: `-f` for “force” and `--rdonly` for read-only. The file system must remember if the read-only option is present.

`replyHandler`  

A block or closure that your implementation invokes when it finishes setting up or encounters an error. Pass a subclass of `FSVolume` as the first parameter if loading succeeds. If loading fails, pass an error as the second parameter.

## Discussion

Implement this method by inspecting the provided resource and verifying it uses a supported format. If the resource does use a supported format, create a subclass of `FSVolume`, clear the container error state, and invoke the `reply` callback, passing your volume as a parameter. If loading can’t proceed, invoke `reply` and send an appropriate error as the second parameter.

## See Also

### Loading and unloading resources

func unloadResource(resource: FSResource, options: FSTaskOptions, replyHandler: ((any Error)?) -> Void)

Requests that the file system unload the specified resource.

**Required**

func didFinishLoading()

Notifies you that the system finished loading your file system extension.

