

- Foundation
- NSCoder
-  decodeUIOffset(forKey:) 

Instance Method

# decodeUIOffset(forKey:)

Decodes and returns the UIKit offset structure associated with the specified key in the coder’s archive.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decodeUIOffset(forKey key: String) -> UIOffset
```

## Parameters 

`key`  

The key that identifies the offset.

## Return Value

The offset data.

## Discussion

Use this method to decode offset information that was previously encoded using the encode(_:forKey:) method.

## See Also

### Related Documentation

func encode(UIOffset, forKey: String)

Encodes offset data and associates it with the specified key in the coder’s archive.

### Decoding Geometry-Based Data

func decodeCGAffineTransform(forKey: String) -> CGAffineTransform

Decodes and returns the Core Graphics affine transform structure associated with the specified key in the coder’s archive.

func decodeCGPoint(forKey: String) -> CGPoint

Decodes and returns the Core Graphics point structure associated with the specified key in the coder’s archive.

func decodeCGRect(forKey: String) -> CGRect

Decodes and returns the Core Graphics rectangle structure associated with the specified key in the coder’s archive.

func decodeCGSize(forKey: String) -> CGSize

Decodes and returns the Core Graphics size structure associated with the specified key in the coder’s archive.

func decodeCGVector(forKey: String) -> CGVector

Decodes and returns the Core Graphics vector data associated with the specified key in the coder’s archive.

func decodeDirectionalEdgeInsets(forKey: String) -> NSDirectionalEdgeInsets

Decodes and returns the UIKit directional edge insets structure associated with the specified key in the coder’s archive.

func decodeUIEdgeInsets(forKey: String) -> UIEdgeInsets

Decodes and returns the UIKit edge insets structure associated with the specified key in the coder’s archive.

