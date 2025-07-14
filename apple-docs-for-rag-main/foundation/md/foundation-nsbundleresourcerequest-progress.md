

- Foundation
- NSBundleResourceRequest
-  progress 

Instance Property

# progress

A reference to the progress object associated with the specified resource request. (read-only)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var progress: Progress { get }
```

## Discussion

This Progress object will begin updating after beginAccessingResources(completionHandler:) is called.

## See Also

### Related Documentation

func beginAccessingResources(completionHandler: ((any Error)?) -> Void)

Requests access to the resources marked with the managed tags. If any of the resources are not on the device, they are requested from the App Store.

