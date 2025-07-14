

- Foundation
- NSCoder
-  decodeTimeMapping(forKey:) 

Instance Method

# decodeTimeMapping(forKey:)

Returns the Core Media time mapping structure associated with a given key.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func decodeTimeMapping(forKey key: String) -> CMTimeMapping
```

## Parameters 

`key`  

The key for a `CMTimeMapping` structure encoded in the receiver.

## Return Value

The `CMTimeMapping` structure associated with `key` in the archive.

## See Also

### Related Documentation

func encode(CMTimeMapping, forKey: String)

Encodes a given Core Media time mapping structure and associates it with a specified key.

### Decoding Core Media Time Structures

func decodeTime(forKey: String) -> CMTime

Returns the Core Media time structure associated with a given key.

func decodeTimeRange(forKey: String) -> CMTimeRange

Returns the Core Media time range structure associated with a given key.

