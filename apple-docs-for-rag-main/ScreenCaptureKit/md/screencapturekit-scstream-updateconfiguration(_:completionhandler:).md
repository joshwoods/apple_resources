

- ScreenCaptureKit
- SCStream
-  updateConfiguration(\_:completionHandler:) 

Instance Method

# updateConfiguration(\_:completionHandler:)

Updates the stream with a new configuration.

Mac Catalyst 18.2+macOS 12.3+

``` source
func updateConfiguration(
    _ streamConfig: SCStreamConfiguration,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func updateConfiguration(_ streamConfig: SCStreamConfiguration) async throws
```

## Parameters 

`streamConfig`  

An object that provides the updated stream configuration.

`completionHandler`  

A completion handler the system calls when this method completes. It includes an error if the update fails.

## See Also

### Updating stream configuration

func updateContentFilter(SCContentFilter, completionHandler: (((any Error)?) -> Void)?)

Updates the stream by applying a new content filter.

