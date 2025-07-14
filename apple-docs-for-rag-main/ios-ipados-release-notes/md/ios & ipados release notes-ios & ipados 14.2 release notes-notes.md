

- iOS &amp; iPadOS Release Notes
-  iOS & iPadOS 14.2 Release Notes 

Article

# iOS & iPadOS 14.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The iOS & iPadOS 14.2 SDK provides support to develop apps for iPhone, iPad, and iPod touch devices running iOS & iPadOS 14.2. The SDK comes bundled with Xcode 12.2, available from the Mac App Store. For information on the compatibility requirements for Xcode 12.2, see Xcode 12.2 Release Notes.

### Core Media

#### New Features

- Support for multiple concurrent AVURLAsset instances on offline HLS filesystem URLs has been improved.

- You can now use multiple concurrent AVPlayerItem objects and other AVFoundation objects on offline HLS assets with completed AVMediaSelection objects without triggering network reads.

- The progress indicator logic of AVMediaSelection ordering for AVAggregateAssetDownloadTask has been improved. (64551736)

### Intercom

#### Resolved Issues

- You can now play and reply to Intercom notifications. (70470421)

### SKAdNetwork

#### Known Issues

- To receive a postback from devices running iOS 14 or later, generate signatures using signature version 2.0 or later. Version 1.0 signatures don’t result in a postback on iOS 14 and later, even if the advertised app is installed and launched. (71474331)

## See Also

### iOS &amp; iPadOS 14

iOS & iPadOS 14.7 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.5.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14 Release Notes

Update your apps to use new features, and test your apps against API changes.

