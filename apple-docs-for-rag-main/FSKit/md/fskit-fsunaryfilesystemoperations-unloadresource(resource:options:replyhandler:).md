

- FSKit
- FSUnaryFileSystemOperations
-  unloadResource(resource:options:replyHandler:) 

Instance Method

# unloadResource(resource:options:replyHandler:)

Requests that the file system unload the specified resource.

macOS 15.4+

``` source
func unloadResource(
    resource: FSResource,
    options: FSTaskOptions,
    replyHandler reply: @escaping ((any Error)?) -> Void
)
```

``` source
func unloadResource(
    resource: FSResource,
    options: FSTaskOptions
) async throws
```

**Required**

## Parameters 

`resource`  

An FSResource to unload.

`options`  

An FSTaskOptions object specifying options to apply when unloading the resource.

`reply`  

A block or closure that your implementation invokes when it finishes unloading or encounters an error. If unloading fails, pass an error as the parameter to describe the problem. Otherwise, pass `nil`.

## See Also

### Loading and unloading resources

func loadResource(resource: FSResource, options: FSTaskOptions, replyHandler: (FSVolume?, (any Error)?) -> Void)

Requests that the file system load a resource and present it as a volume.

**Required**

func didFinishLoading()

Notifies you that the system finished loading your file system extension.

