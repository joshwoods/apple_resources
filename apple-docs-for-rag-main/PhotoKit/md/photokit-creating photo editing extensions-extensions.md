

- PhotoKit
-  Creating Photo Editing Extensions 

Article

# Creating Photo Editing Extensions

Provide custom functionality in the Photos app by bundling an app extension.

iOS 8.0+iPadOS 8.0+macOS 10.11+visionOS 1.0+

## Overview

You can incorporate your app’s features directly into the Photos app in iOS or macOS by building an app extension. A photo-editing app extension can enable people to edit media, apply your app’s filter effects, build slideshows, books, or custom content, such as a collage, right in Photos app using code that you supply.

## Implement and bundle the app extension

Adopt the PHContentEditingController protocol to create an app extension that adds to the photo editing options and capabilities in the Photos app. Creating such an extension also requires using the following classes from the Photos framework:

- PHContentEditingInput—To reference the photo or video to be edited

- PHContentEditingOutput—To save the results of an edit

- PHAdjustmentData—To describe an edit operation

Include the app extension in your app bundle and the system installs it in Photos at the same time someone installs your app.

Note

If your app runs on a platform other than those listed above, the platform ignores your app extension.

## See Also

### Articles

Delivering an Enhanced Privacy Experience in Your Photos App

Adopt the latest privacy enhancements to deliver advanced user-privacy controls.

Fetching Objects and Requesting Changes

Get assets, asset collections, and collection lists matching a specified query.

Loading and Caching Assets and Thumbnails

Request image, video, or Live Photos content, and cache for quick reuse.

Displaying Live Photos

Provide the same interactive playback of Live Photos as in the iOS Photos app.

