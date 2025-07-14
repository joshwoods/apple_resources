

- Foundation
- Bundle
-  setPreservationPriority(\_:forTags:) 

Instance Method

# setPreservationPriority(\_:forTags:)

A hint to the system of the relative order for purging tagged sets of resources in the bundle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setPreservationPriority(
    _ priority: Double,
    forTags tags: Set
)
```

## Parameters 

`priority`  

A number specifying the relative priority of preserving the resources in the group specified by `tag`.

Possible values are between `0.0` and `1.0`. The default is `0.0`. The system will attempt to purge resources with lower priorities first.

`tags`  

A set of tag names specifying resources stored in the bundle. Must not be `nil`. An exception is thrown if any of the tags in the set do not exist in your app.

## See Also

### Managing Preservation Priority for On Demand Resources

func preservationPriority(forTag: String) -> Double

Returns the current preservation priority for the specified tag.

