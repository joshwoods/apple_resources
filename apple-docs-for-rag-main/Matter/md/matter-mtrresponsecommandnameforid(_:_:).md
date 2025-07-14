

- Matter
-  MTRResponseCommandNameForID(\_:\_:) 

Function

# MTRResponseCommandNameForID(\_:\_:)

Resolve Matter response (server to client) command IDs into a descriptive string.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func MTRResponseCommandNameForID(
    _ clusterID: MTRClusterIDType,
    _ commandID: MTRCommandIDType
) -> String!
```

## Discussion

For unknown IDs, a string ‘\’ (if the cluster ID is not known) or ‘\’ (if the cluster ID is known but the command ID is not known) will be returned.

