

- Foundation
-  NSBundleResourceRequestLoadingPriorityUrgent 

Global Variable

# NSBundleResourceRequestLoadingPriorityUrgent

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSBundleResourceRequestLoadingPriorityUrgent: Double
```

## Discussion

A special value for loading priority informing the system that the user cannot continue until the resources marked with the tags managed by the request are downloaded. The system will dedicate the maximum amount of capacity to completing the resource request.

## See Also

### Setting the Download Priority

var loadingPriority: Double

A hint to the system of the relative priority of the resource request.

