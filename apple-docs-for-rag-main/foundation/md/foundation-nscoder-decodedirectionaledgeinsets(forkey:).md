

- Foundation
- NSCoder
-  decodeDirectionalEdgeInsets(forKey:) 

Instance Method

# decodeDirectionalEdgeInsets(forKey:)

Decodes and returns the UIKit directional edge insets structure associated with the specified key in the coder’s archive.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func decodeDirectionalEdgeInsets(forKey key: String) -> NSDirectionalEdgeInsets
```

## Parameters 

`key`  

The key that identifies the edge insets.

## Discussion

Use this method to decode edge inset information that was previously encoded using the encode(_:forKey:) method.

## See Also

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

func decodeUIEdgeInsets(forKey: String) -> UIEdgeInsets

Decodes and returns the UIKit edge insets structure associated with the specified key in the coder’s archive.

func decodeUIOffset(forKey: String) -> UIOffset

Decodes and returns the UIKit offset structure associated with the specified key in the coder’s archive.

