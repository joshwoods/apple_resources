

- Core Services
- OS Services
- Identity Services
- CSIdentityQueryClientContext
-  init(version:info:retainInfo:releaseInfo:copyInfoDescription:receiveEvent:) 

Initializer

# init(version:info:retainInfo:releaseInfo:copyInfoDescription:receiveEvent:)

Mac Catalyst 13.0+macOS 10.9+Xcode 9.0+

``` source
init(
    version: CFIndex,
    info: UnsafeMutableRawPointer!,
    retainInfo: CFAllocatorRetainCallBack!,
    releaseInfo: CFAllocatorReleaseCallBack!,
    copyInfoDescription: CFAllocatorCopyDescriptionCallBack!,
    receiveEvent: CSIdentityQueryReceiveEventCallback!
)
```

