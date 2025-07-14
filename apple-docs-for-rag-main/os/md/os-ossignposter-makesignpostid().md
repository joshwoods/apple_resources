

- os
- OSSignposter
-  makeSignpostID() 

Instance Method

# makeSignpostID()

Returns an identifier that’s unique within the scope of the signposter.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func makeSignpostID() -> OSSignpostID
```

## Return Value

A signpost ID that you use to match an interval’s signposts.

## Mentioned in 

Recording Performance Data

## Discussion

The signposter uses a signpost ID to pair the beginning and the end of a signposted interval, which is necessary because multiple intervals with the same configuration and scope can be in-flight simultaneously.

Use this method instead of init(log:).

## See Also

### Generating Signpost IDs

func makeSignpostID(from: AnyObject) -> OSSignpostID

Returns an identifier that the signposter derives from the specified object.

struct OSSignpostID

An identifier that disambiguates signposted intervals.

