

- os
- OSSignposter
-  makeSignpostID(from:) 

Instance Method

# makeSignpostID(from:)

Returns an identifier that the signposter derives from the specified object.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func makeSignpostID(from object: AnyObject) -> OSSignpostID
```

## Parameters 

`object`  

The object the signposter uses to match the begin and end calls of a signposted interval.

## Return Value

A signpost ID that you use to match an interval’s signposts.

## Discussion

Warning

Don’t use this method to generate an identifier for a signposted interval that crosses process boundaries. Instead, use the makeSignpostID() method.

The signposter uses a signpost ID to pair the beginning and the end of a signposted interval, which is necessary because multiple intervals with the same configuration and scope can be in-flight simultaneously.

Use this method instead of init(log:object:).

## See Also

### Generating Signpost IDs

func makeSignpostID() -> OSSignpostID

Returns an identifier that’s unique within the scope of the signposter.

struct OSSignpostID

An identifier that disambiguates signposted intervals.

