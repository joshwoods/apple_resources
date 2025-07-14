

- AVFoundation
- AVContentKeySession
-  init(keySystem:storageDirectoryAt:) 

Initializer

# init(keySystem:storageDirectoryAt:)

Creates a content key session to manage a collection of content decryption keys; points to a directory that stores abnormal session termination reports.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
convenience init(
    keySystem: AVContentKeySystem,
    storageDirectoryAt storageURL: URL
)
```

## Parameters 

`keySystem`  

A valid key system used to retrieve keys.

`storageURL`  

A URL that points to a writable directory. The session uses the directory to facilitate expired session reports after an abnormal session termination.

## Return Value

Returns a new AVContentKeySession instance.

## Discussion

The `AVContentKeySession` instance returned is capable of managing a collection of content decryption keys that correspond to the input key system. An invalidArgumentException is raised when the value of `keySystem` is unsupported.

## See Also

### Creating a Session

convenience init(keySystem: AVContentKeySystem)

Creates a content key session to manage a collection of content decryption keys.

