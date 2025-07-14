

- ScreenCaptureKit
- SCContentSharingPickerObserver
-  contentSharingPicker(\_:didUpdateWith:for:) 

Instance Method

# contentSharingPicker(\_:didUpdateWith:for:)

Tells the observer that a sharing picker updated the content filter for a stream.

Mac Catalyst 18.2+macOS 14.0+

``` source
func contentSharingPicker(
    _ picker: SCContentSharingPicker,
    didUpdateWith filter: SCContentFilter,
    for stream: SCStream?
)
```

**Required**

## Parameters 

`picker`  

The content-sharing picker that sent this event.

`filter`  

The new filter applied to streaming content.

`stream`  

The changed stream, if any.

## See Also

### Observing events

func contentSharingPicker(SCContentSharingPicker, didCancelFor: SCStream?)

Tells the observer that a sharing picker canceled selection for a stream.

**Required**

