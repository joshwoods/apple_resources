

- Foundation
- NSBundleResourceRequest
-  loadingPriority 

Instance Property

# loadingPriority

A hint to the system of the relative priority of the resource request.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var loadingPriority: Double { get set }
```

## Discussion

Possible values are between `0.0` and `1.0` or the special constant NSBundleResourceRequestLoadingPriorityUrgent. The default is `0.5`. The system will attempt to give higher priority to requests with higher values. You can change the priority at any time, including during downloading of the managed resources.

## See Also

### Setting the Download Priority

let NSBundleResourceRequestLoadingPriorityUrgent: Double

