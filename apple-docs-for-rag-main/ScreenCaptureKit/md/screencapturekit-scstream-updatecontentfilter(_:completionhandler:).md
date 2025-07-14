

- ScreenCaptureKit
- SCStream
-  updateContentFilter(\_:completionHandler:) 

Instance Method

# updateContentFilter(\_:completionHandler:)

Updates the stream by applying a new content filter.

Mac Catalyst 18.2+macOS 12.3+

``` source
func updateContentFilter(
    _ contentFilter: SCContentFilter,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func updateContentFilter(_ contentFilter: SCContentFilter) async throws
```

## Parameters 

`contentFilter`  

The content filter to apply.

`completionHandler`  

A completion handler the system calls when this method completes. It includes an error if the update fails.

## See Also

### Updating stream configuration

func updateConfiguration(SCStreamConfiguration, completionHandler: (((any Error)?) -> Void)?)

Updates the stream with a new configuration.

