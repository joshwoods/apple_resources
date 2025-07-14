

- Matter
-  MTREventNameForID(\_:\_:) 

Function

# MTREventNameForID(\_:\_:)

Resolve Matter event IDs into a descriptive string.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func MTREventNameForID(
    _ clusterID: MTRClusterIDType,
    _ eventID: MTREventIDType
) -> String!
```

## Discussion

For unknown IDs, a string ‘\’ (if the cluster ID is not known) or ‘\’ (if the cluster ID is known but the event ID is not known) will be returned.

