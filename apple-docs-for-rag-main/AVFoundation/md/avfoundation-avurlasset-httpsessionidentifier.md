

- AVFoundation
- AVURLAsset
-  httpSessionIdentifier 

Instance Property

# httpSessionIdentifier

A session identifier that the asset sends in HTTP requests that it makes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var httpSessionIdentifier: UUID { get }
```

## Discussion

The asset uses this value to set as the `X-Playback-Session-Id` header of HTTP requests that it creates.

Note

Copies of an AVURLAsset have the same session identifier as the original asset.

