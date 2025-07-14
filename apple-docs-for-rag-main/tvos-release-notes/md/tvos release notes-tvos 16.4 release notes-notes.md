

- tvOS Release Notes
-  tvOS 16.4 Release Notes 

Article

# tvOS 16.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The tvOS 16.4 SDK provides support to develop tvOS apps for Apple TV devices running tvOS 16.4. The SDK comes bundled with Xcode 14.3, available from the Mac App Store. For information on the compatibility requirements for Xcode 14.3, see Xcode 14.3 Release Notes.

### Home

#### New Features

- Both manual and automatic Software Update support is now available for Matter Accessories. (102727759)

### SwiftUI

#### Resolved Issues

- Fixed: `ScrollView` has improved support for right to left languages by default. If you have a `ScrollView` that shouldn’t change its behavior in right to left languages, use the `.environment(\.layoutDirection, .leftToRight)` modifier to ensure the `ScrollView` always sees a left to right layout direction. (65108729)

- Fixed: Search scopes are now supported on tvOS. (84039097)

- Fixed: Presentations in SwiftUI using the ‘sheet’ or ‘fullScreenCover’ modifier can now be dynamically presented again while a dismiss animation is in progress. Previously, attempting to present again in this case would do nothing.

  Note: A data race in app code that was previously ignored might cause a sheet to be presented again with this change. If this happens, check that your state isn’t triggering a new presentation. (101487810)

## See Also

### tvOS 16

tvOS 16.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 16.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 16.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 16.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 16.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 16 Release Notes

Update your apps to use new features, and test your apps against API changes.

