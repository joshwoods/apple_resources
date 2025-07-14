

- PhotoKit
-  Fetching Objects and Requesting Changes 

Article

# Fetching Objects and Requesting Changes

Get assets, asset collections, and collection lists matching a specified query.

## Overview

Instances of the model classes PHAsset, PHAssetCollection, and PHCollectionList represent the items a user works with in the Photos app:

- **Assets**: Images, videos, and Live Photos

- **Collections of assets**: Albums or Moments

- **Lists of collections**: Album folders or Moment clusters

Instances of these classes are read-only and immutable, and contain only metadata. Use these classes to fetch a set of objects matching a specified query.

### Commit Change Requests to the Shared Photo Library

Fetch assets and collections you’re interested in, and use those objects to fetch the raw data you need to reference or edit. To make changes, create change request objects and explicitly commit them to the shared PHPhotoLibrary object. This architecture makes it easy, safe, and efficient to work with the same assets from multiple threads or multiple apps and app extensions.

### Handle Special Assets

PhotoKit supports a number of Photos app features for working directly with a user’s Photos library. For example, Live Photos are special assets with additional data that your app can display differently, as a video or sequence of frames.

Use the PHCollectionList class to find assets corresponding to the Moments hierarchy in the Photos App. Lists of collections are read-only, immutable, and contain only metadata. Use the PHAsset class to identify burst photos, Live Photos, panoramic photos, and high-frame-rate videos. When iCloud Photos is enabled, assets and collections in the Photos framework reflect content available across all devices on the same iCloud account.

For more information about Live Photos, see Displaying Live Photos.

## See Also

### Articles

Delivering an Enhanced Privacy Experience in Your Photos App

Adopt the latest privacy enhancements to deliver advanced user-privacy controls.

Loading and Caching Assets and Thumbnails

Request image, video, or Live Photos content, and cache for quick reuse.

Displaying Live Photos

Provide the same interactive playback of Live Photos as in the iOS Photos app.

Creating Photo Editing Extensions

Provide custom functionality in the Photos app by bundling an app extension.

