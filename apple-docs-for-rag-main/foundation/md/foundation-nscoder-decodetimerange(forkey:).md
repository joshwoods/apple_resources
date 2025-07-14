

- Foundation
- NSCoder
-  decodeTimeRange(forKey:) 

Instance Method

# decodeTimeRange(forKey:)

Returns the Core Media time range structure associated with a given key.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func decodeTimeRange(forKey key: String) -> CMTimeRange
```

## Parameters 

`key`  

The key for a `CMTimeRange` structure encoded in the receiver.

## Return Value

The `CMTimeRange` structure associated with `key` in the archive.

## See Also

### Related Documentation

func encode(CMTimeRange, forKey: String)

Encodes a given Core Media time range structure and associates it with a specified key.

### Decoding Core Media Time Structures

func decodeTime(forKey: String) -> CMTime

Returns the Core Media time structure associated with a given key.

func decodeTimeMapping(forKey: String) -> CMTimeMapping

Returns the Core Media time mapping structure associated with a given key.

