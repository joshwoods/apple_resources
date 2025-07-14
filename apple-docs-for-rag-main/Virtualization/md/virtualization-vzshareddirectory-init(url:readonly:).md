

- Virtualization
- VZSharedDirectory
-  init(url:readOnly:) 

Initializer

# init(url:readOnly:)

Initialize with a host directory.

macOS 12.0+

``` source
init(
    url: URL,
    readOnly: Bool
)
```

## Parameters 

`url`  

A local file URL to expose to the guest.

`readOnly`  

A Boolean value that indicates whether to expose the directory as read-only to the guest.

## Discussion

