

- Media Player
-  Displaying a media picker from your app 

Article

# Displaying a media picker from your app

Let users choose the music they want to play by displaying a media picker interface from within your app.

## Overview

Add a media picker view controller to your app to enable users to choose music items from their Apple Music library without leaving your app. You can configure the media picker to accept single or multiple items from the user.

Important

Your app’s `Info.plist` file must include the NSAppleMusicUsageDescription key prior to accessing the user’s music library. If that key isn’t present, displaying the media picker causes your app to exit.

### Adopt the Protocol, and Create the System Music Player

To enable your app to respond to user input, adopt the MPMediaPickerControllerDelegate protocol.

```
```

### Add the media picker view controller

Set the media picker view controller as a popover presentation controller when you target an iPad. Set the source view and delegate, and present the media picker. In this example, the media picker allows the user to select multiple items, and the source view is a button object.

```
```

### Add a select music button, and target the previously created function

To create a button that gives the user access to their Apple Music library from within your app:

1.  Add a UIButton object, and name it Select Songs.

2.  Attach restraints to center the button in the display.

3.  Control-drag from the new button object to View Controller in the Outline view, and select `selectSongs:` from the menu that appears.

The Select Songs button is the source view for the media picker that the view controller presents modally. The media picker displays the user’s Apple Music library, which allows them to choose the music they want to play.

### Implement the protocol methods

Implement two methods from the `MPMediaPickerControllerDelegate` protocol: mediaPicker(_:didPickMediaItems:) and mediaPickerDidCancel(_:). Inside these methods, add code to handle the user’s choice of items to create a music queue, and code to dismiss the view controller. The following code shows how to set the music player queue, begin playing the user’s choices, and dismiss the view controller if the user doesn’t choose any media items:

```
```

## See Also

### Related Documentation

Playing audio using the built-in music player

Create a media player inside your app to play audio from the user’s media library.

### Media player user interface

class MPMediaPickerController

A specialized view controller that provides a graphical interface for selecting media items.

class MPVolumeView

A slider control for setting the system audio output volume, and a button for choosing the audio output route.

