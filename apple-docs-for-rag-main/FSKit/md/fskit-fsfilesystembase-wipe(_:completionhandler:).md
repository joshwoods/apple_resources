

- FSKit
- FSFileSystemBase
-  wipe(\_:completionHandler:) 

Instance Method

# wipe(\_:completionHandler:)

Wipes existing file systems on the specified resource.

macOS 15.4+

``` source
func wipe(
    _ resource: FSBlockDeviceResource,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func wipe(_ resource: FSBlockDeviceResource) async throws
```

**Required**

## Parameters 

`resource`  

The FSBlockDeviceResource to wipe.

`completion`  

A block or closure that executes after the wipe operation completes. The completion handler receives a single parameter indicating any error that occurs during the operation. If the value is `nil`, the wipe operation succeeded.

## Discussion

This method wraps the `wipefs` functionality from `libutil`. For more information, see the `man` page for `wipefs`.

