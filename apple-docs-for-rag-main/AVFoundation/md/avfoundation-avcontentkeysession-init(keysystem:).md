

- AVFoundation
- AVContentKeySession
-  init(keySystem:) 

Initializer

# init(keySystem:)

Creates a content key session to manage a collection of content decryption keys.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 7.0+

``` source
convenience init(keySystem: AVContentKeySystem)
```

## Parameters 

`keySystem`  

A valid key system used to retrieve keys.

## Return Value

Returns a new AVContentKeySession instance.

## Discussion

The `AVContentKeySession` instance returned is capable of managing a collection of content decryption keys that correspond to the input key system. An invalidArgumentException is raised when the value of `keySystem` is unsupported.

## See Also

### Creating a Session

convenience init(keySystem: AVContentKeySystem, storageDirectoryAt: URL)

Creates a content key session to manage a collection of content decryption keys; points to a directory that stores abnormal session termination reports.

