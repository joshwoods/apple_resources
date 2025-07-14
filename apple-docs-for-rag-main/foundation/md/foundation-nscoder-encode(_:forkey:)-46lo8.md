

- Foundation
- NSCoder
-  encode(\_:forKey:) 

Instance Method

# encode(\_:forKey:)

Encodes a given Core Media time range structure and associates it with a specified key.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func encode(
    _ timeRange: CMTimeRange,
    forKey key: String
)
```

## Parameters 

`timeRange`  

A `CMTimeRange` structure.

`key`  

The key with which to associate `timeRange` in the archive.

## See Also

### Related Documentation

func decodeTimeRange(forKey: String) -> CMTimeRange

Returns the Core Media time range structure associated with a given key.

### Encoding Core Media Time Structures

func encode(CMTime, forKey: String)

Encodes a given Core Media time structure and associates it with a specified key.

func encode(CMTimeMapping, forKey: String)

Encodes a given Core Media time mapping structure and associates it with a specified key.

