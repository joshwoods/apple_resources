

- PhotoKit
-  Displaying Live Photos 

Article

# Displaying Live Photos

Provide the same interactive playback of Live Photos as in the iOS Photos app.

## Overview

The PHLivePhotoView class provides a way to display Live Photos—pictures, taken on compatible hardware, that include motion and sound from the moments just before and after their capture. A Live Photo view provides the same interactive playback features found in the Photos app.

In iOS and tvOS, you can fetch Live Photo objects to display in a Live Photo view with the PHLivePhoto class in the Photos framework. In macOS, the PHLivePhoto class provides access to Live Photos being edited in a photo editing extension for the Photos app.

To display Live Photo content on the web, use the LivePhotosKit JS framework.

### Control Live Photo Playback

After obtaining a PHLivePhoto object, use a Live Photo view to display the photo and control playback of its motion and sound content. In iOS and tvOS, you can obtain Live Photos from the user’s photo library using the UIImagePickerController, PHAsset, and PHImageManager classes, or by creating one from asset resources exported from a photo library. In macOS, Live Photos are available only when editing Live Photo content in a photo editing extension that runs in the Photos app—see the PHContentEditingInput class to access Live Photos in an editing session.

Note

For guidance on how to integrate Live Photos with your app’s user experience, see Live Photos in iOS Human Interface Guidelines.

By default, a Live Photo view uses its own gesture recognizer to allow the user to play the motion and sound content of a Live Photo with the same interactions and visual effects seen in the Photos app. To customize this gesture recognizer—for example, to install it on a different view for proper event handling in your app’s view hierarchy—use the playbackGestureRecognizer property.

Typically, an app doesn’t need to directly control Live Photo playback. In some situations, however, it can be useful to briefly animate the view to indicate to the user that a picture is a Live Photo. To do this, use the startPlayback(with:) method with the PHLivePhotoViewPlaybackStyle.hint option.

## See Also

### Articles

Delivering an Enhanced Privacy Experience in Your Photos App

Adopt the latest privacy enhancements to deliver advanced user-privacy controls.

Fetching Objects and Requesting Changes

Get assets, asset collections, and collection lists matching a specified query.

Loading and Caching Assets and Thumbnails

Request image, video, or Live Photos content, and cache for quick reuse.

Creating Photo Editing Extensions

Provide custom functionality in the Photos app by bundling an app extension.

