

- Foundation
- NSCoder
-  encode(\_:forKey:) 

Instance Method

# encode(\_:forKey:)

Encodes directional edge inset data and associates it with the specified key in the coder’s archive.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func encode(
    _ insets: NSDirectionalEdgeInsets,
    forKey key: String
)
```

## Parameters 

`insets`  

The edge insets data to encode.

`key`  

The key identifying the data.

## Discussion

When decoding the data from the archive, you pass the value in the key parameter to the corresponding decodeDirectionalEdgeInsets(forKey:) method to retrieve the data.

## See Also

### Encoding Geometry-Based Data

func encode(CGAffineTransform, forKey: String)

Encodes an affine transform and associates it with the specified key in the receiver’s archive.

func encode(CGPoint, forKey: String)

Encodes a point and associates it with the specified key in the receiver’s archive.

func encode(CGRect, forKey: String)

Encodes a rectangle and associates it with the specified key in the receiver’s archive.

func encode(CGSize, forKey: String)

Encodes size information and associates it with the specified key in the coder’s archive.

func encode(CGVector, forKey: String)

Encodes vector data and associates it with the specified key in the coder’s archive.

func encode(UIEdgeInsets, forKey: String)

Encodes edge inset data and associates it with the specified key in the coder’s archive.

func encode(UIOffset, forKey: String)

Encodes offset data and associates it with the specified key in the coder’s archive.

