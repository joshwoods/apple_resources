

- Media Player
- MPMediaPickerControllerDelegate
-  mediaPicker(\_:didPickMediaItems:) 

Instance Method

# mediaPicker(\_:didPickMediaItems:)

A method that the system calls when a user selects a set of media items.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+

``` source
optional func mediaPicker(
    _ mediaPicker: MPMediaPickerController,
    didPickMediaItems mediaItemCollection: MPMediaItemCollection
)
```

## Parameters 

`mediaPicker`  

The media item picker to dismiss.

`mediaItemCollection`  

The selected media items.

## Mentioned in 

Displaying a media picker from your app

## See Also

### Related Documentation

iPod Library Access Programming Guide

### Responding to user actions

func mediaPickerDidCancel(MPMediaPickerController)

A method that the system calls when a user taps Cancel to dismiss a media item picker.

