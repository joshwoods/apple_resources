

- Foundation
- Bundle
-  preservationPriority(forTag:) 

Instance Method

# preservationPriority(forTag:)

Returns the current preservation priority for the specified tag.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func preservationPriority(forTag tag: String) -> Double
```

## Parameters 

`tag`  

A string specifying the identifier for a group of related resources. An exception is thrown if `tag` does not exist in your app.

## Return Value

The preservation priority for the specified `tag`. Possible values are between `0.0` and `1.0`

## See Also

### Managing Preservation Priority for On Demand Resources

func setPreservationPriority(Double, forTags: Set&lt;String>)

A hint to the system of the relative order for purging tagged sets of resources in the bundle.

