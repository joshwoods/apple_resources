

- Foundation
- NSCoder
-  decodeCGVector(forKey:) 

Instance Method

# decodeCGVector(forKey:)

Decodes and returns the Core Graphics vector data associated with the specified key in the coder’s archive.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decodeCGVector(forKey key: String) -> CGVector
```

## Parameters 

`key`  

The key that identifies the vector.

## Return Value

The vector data.

## Discussion

Use this method to decode vector information that was previously encoded using the encode(_:forKey:) method.

## See Also

### Related Documentation

func encode(CGVector, forKey: String)

Encodes vector data and associates it with the specified key in the coder’s archive.

### Decoding Geometry-Based Data

func decodeCGAffineTransform(forKey: String) -> CGAffineTransform

Decodes and returns the Core Graphics affine transform structure associated with the specified key in the coder’s archive.

func decodeCGPoint(forKey: String) -> CGPoint

Decodes and returns the Core Graphics point structure associated with the specified key in the coder’s archive.

func decodeCGRect(forKey: String) -> CGRect

Decodes and returns the Core Graphics rectangle structure associated with the specified key in the coder’s archive.

func decodeCGSize(forKey: String) -> CGSize

Decodes and returns the Core Graphics size structure associated with the specified key in the coder’s archive.

func decodeDirectionalEdgeInsets(forKey: String) -> NSDirectionalEdgeInsets

Decodes and returns the UIKit directional edge insets structure associated with the specified key in the coder’s archive.

func decodeUIEdgeInsets(forKey: String) -> UIEdgeInsets

Decodes and returns the UIKit edge insets structure associated with the specified key in the coder’s archive.

func decodeUIOffset(forKey: String) -> UIOffset

Decodes and returns the UIKit offset structure associated with the specified key in the coder’s archive.

