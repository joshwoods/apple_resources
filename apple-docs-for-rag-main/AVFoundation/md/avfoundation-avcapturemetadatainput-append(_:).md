

- AVFoundation
- AVCaptureMetadataInput
-  append(\_:) 

Instance Method

# append(\_:)

Provides metadata to the capture session.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func append(_ metadata: AVTimedMetadataGroup) throws
```

## Parameters 

`metadata`  

A timed group of metadata. To denote a period of no metadata, pass an empty AVTimedMetadataGroup.

