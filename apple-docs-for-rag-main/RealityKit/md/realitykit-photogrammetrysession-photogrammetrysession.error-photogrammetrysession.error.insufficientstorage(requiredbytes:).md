

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Error
-  PhotogrammetrySession.Error.insufficientStorage(requiredBytes:) 

Case

# PhotogrammetrySession.Error.insufficientStorage(requiredBytes:)

An error that indicates insufficient storage space.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
case insufficientStorage(requiredBytes: Int64)
```

## Discussion

This error occurs when there is not enough available storage, and the system estimates that it needs `requiredBytes` of storage.

