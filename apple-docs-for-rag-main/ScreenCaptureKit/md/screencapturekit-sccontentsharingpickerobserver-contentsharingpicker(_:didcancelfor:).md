

- ScreenCaptureKit
- SCContentSharingPickerObserver
-  contentSharingPicker(\_:didCancelFor:) 

Instance Method

# contentSharingPicker(\_:didCancelFor:)

Tells the observer that a sharing picker canceled selection for a stream.

Mac Catalyst 18.2+macOS 14.0+

``` source
func contentSharingPicker(
    _ picker: SCContentSharingPicker,
    didCancelFor stream: SCStream?
)
```

**Required**

## Parameters 

`picker`  

The content-sharing picker that sent this event.

`stream`  

The canceled stream, if any.

## See Also

### Observing events

func contentSharingPicker(SCContentSharingPicker, didUpdateWith: SCContentFilter, for: SCStream?)

Tells the observer that a sharing picker updated the content filter for a stream.

**Required**

