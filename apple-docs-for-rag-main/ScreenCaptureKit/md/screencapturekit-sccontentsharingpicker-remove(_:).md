

- ScreenCaptureKit
- SCContentSharingPicker
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes an observer instance from the content-sharing picker.

Mac Catalyst 18.2+macOS 14.0+

``` source
func remove(_ observer: any SCContentSharingPickerObserver)
```

## Parameters 

`observer`  

The observer instance to remove.

## See Also

### Manage observers

func add(any SCContentSharingPickerObserver)

Adds an observer instance to notify of changes in the content-sharing picker.

