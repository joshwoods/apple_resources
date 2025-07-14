

- AVFoundation
- AVPartialAsyncProperty
-  hasProtectedContent 

Type Property

# hasProtectedContent

A Boolean value that indicates whether the asset contains protected content.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var hasProtectedContent: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

Assets that contain protected content may not be playable without successful authorization, even if the value of its isPlayable property is true.

