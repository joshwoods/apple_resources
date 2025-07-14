

- AVFoundation
- AVPartialAsyncProperty
-  trackGroups 

Type Property

# trackGroups

The track groups an asset contains.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var trackGroups: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

The value is an empty array if the asset has no track groups.

