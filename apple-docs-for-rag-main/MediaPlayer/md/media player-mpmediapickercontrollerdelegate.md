

- Media Player
-  MPMediaPickerControllerDelegate 

Protocol

# MPMediaPickerControllerDelegate

The protocol you implement so that a media item picker can respond to a user making media item selections.

iOSiPadOSMac Catalyst

``` source
protocol MPMediaPickerControllerDelegate : NSObjectProtocol
```

## Mentioned in 

Displaying a media picker from your app

## Overview

The delegate for a media item picker can respond to a user making media item selections. The delegate is also responsible for dismissing the media item picker from the parent view controller. The methods in this protocol are optional.

MPMediaItem describes the media items and MPMediaPickerController describes the media item pickers.

## Topics

### Responding to user actions

func mediaPicker(MPMediaPickerController, didPickMediaItems: MPMediaItemCollection)

A method that the system calls when a user selects a set of media items.

func mediaPickerDidCancel(MPMediaPickerController)

A method that the system calls when a user taps Cancel to dismiss a media item picker.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to media item picker selections

var delegate: (any MPMediaPickerControllerDelegate)?

The delegate for a media item picker.

