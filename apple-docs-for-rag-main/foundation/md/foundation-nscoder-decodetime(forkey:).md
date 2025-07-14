

- Foundation
- NSCoder
-  decodeTime(forKey:) 

Instance Method

# decodeTime(forKey:)

Returns the Core Media time structure associated with a given key.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func decodeTime(forKey key: String) -> CMTime
```

## Parameters 

`key`  

The key for a `CMTime` structure encoded in the receiver.

## Return Value

The `CMTime` structure associated with `key` in the archive.

## See Also

### Related Documentation

func encode(CMTime, forKey: String)

Encodes a given Core Media time structure and associates it with a specified key.

### Decoding Core Media Time Structures

func decodeTimeRange(forKey: String) -> CMTimeRange

Returns the Core Media time range structure associated with a given key.

func decodeTimeMapping(forKey: String) -> CMTimeMapping

Returns the Core Media time mapping structure associated with a given key.

