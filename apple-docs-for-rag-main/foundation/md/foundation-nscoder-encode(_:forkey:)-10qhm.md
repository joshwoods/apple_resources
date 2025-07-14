

- Foundation
- NSCoder
-  encode(\_:forKey:) 

Instance Method

# encode(\_:forKey:)

Encodes a rectangle and associates it with the specified key in the receiver’s archive.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encode(
    _ rect: CGRect,
    forKey key: String
)
```

## Parameters 

`rect`  

The rectangle to encode.

`key`  

The key identifying the data.

## Discussion

When decoding the data from the archive, you pass the value in the `key` parameter to the corresponding decodeCGRect(forKey:) method to retrieve the data.

## See Also

### Related Documentation

func decodeCGRect(forKey: String) -> CGRect

Decodes and returns the Core Graphics rectangle structure associated with the specified key in the coder’s archive.

### Encoding Geometry-Based Data

func encode(CGAffineTransform, forKey: String)

Encodes an affine transform and associates it with the specified key in the receiver’s archive.

func encode(CGPoint, forKey: String)

Encodes a point and associates it with the specified key in the receiver’s archive.

func encode(CGSize, forKey: String)

Encodes size information and associates it with the specified key in the coder’s archive.

func encode(CGVector, forKey: String)

Encodes vector data and associates it with the specified key in the coder’s archive.

func encode(NSDirectionalEdgeInsets, forKey: String)

Encodes directional edge inset data and associates it with the specified key in the coder’s archive.

func encode(UIEdgeInsets, forKey: String)

Encodes edge inset data and associates it with the specified key in the coder’s archive.

func encode(UIOffset, forKey: String)

Encodes offset data and associates it with the specified key in the coder’s archive.

