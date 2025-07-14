

- AVFoundation
- AVPartialAsyncProperty
-  variants 

Type Property

# variants

An array of variants that an asset contains.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var variants: AVAsyncProperty { get }
```

Available when `Root` inherits `AVURLAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

Some variants may not be playable according to the current device configuration.

