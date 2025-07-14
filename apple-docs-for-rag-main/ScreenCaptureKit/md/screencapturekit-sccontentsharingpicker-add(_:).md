

- ScreenCaptureKit
- SCContentSharingPicker
-  add(\_:) 

Instance Method

# add(\_:)

Adds an observer instance to notify of changes in the content-sharing picker.

Mac Catalyst 18.2+macOS 14.0+

``` source
func add(_ observer: any SCContentSharingPickerObserver)
```

## Parameters 

`observer`  

The observer instance to send notifications to.

## See Also

### Manage observers

func remove(any SCContentSharingPickerObserver)

Removes an observer instance from the content-sharing picker.

