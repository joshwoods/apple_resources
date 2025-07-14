

- Foundation
- NSCoder
-  encode(\_:forKey:) 

Instance Method

# encode(\_:forKey:)

Encodes a given Core Media time structure and associates it with a specified key.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func encode(
    _ time: CMTime,
    forKey key: String
)
```

## Parameters 

`time`  

A `CMTime` structure.

`key`  

The key with which to associate `time` in the archive.

## See Also

### Related Documentation

func decodeTime(forKey: String) -> CMTime

Returns the Core Media time structure associated with a given key.

### Encoding Core Media Time Structures

func encode(CMTimeRange, forKey: String)

Encodes a given Core Media time range structure and associates it with a specified key.

func encode(CMTimeMapping, forKey: String)

Encodes a given Core Media time mapping structure and associates it with a specified key.

