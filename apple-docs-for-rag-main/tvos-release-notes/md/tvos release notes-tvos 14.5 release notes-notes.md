

- tvOS Release Notes
-  tvOS 14.5 Release Notes 

Article

# tvOS 14.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The tvOS 14.5 SDK provides support to develop tvOS apps for Apple TV devices running tvOS 14.5. The SDK comes bundled with Xcode 12.5, available from the Mac App Store. For information on the compatibility requirements for Xcode 12.5, see Xcode 12.5 Release Notes.

### Accessibility

#### New Features

- Many SF Symbols now have default accessibility labels. (70305995)

### Combine

#### Resolved Issues

- Using Published in a subclass of a type conforming to ObservableObject now correctly publishes changes. (70305995)

### SwiftUI

#### New Features

- Added TitleAndIconLabelStyle, a new style for Label views that shows both the title and icon of the label using a system-standard layout. In most cases, labels show both title and icon by default. However, some containers might apply a different default label style to their content, such as only showing icons within toolbars on macOS and iOS. To opt in to showing both the title and the icon, apply the title and icon label style: `Label("Lightning", systemImage: "bolt.fill").labelStyle(TitleAndIconLabelStyle())`. (64646578)

- Types conforming to any style protocol, such as ButtonStyle or ToggleStyle, are now enforced to be value types. Styles must be structures or enumerations, not classes, and conforming a class to a style protocol may trigger an assertion. This is the same restriction that the system has always enforced on types conforming to View. (62886135)

#### Resolved Issues

- You can now apply multiple doc://com.apple.documentation/documentation/swiftui/anyview/sheet(ispresented:ondismiss:content:) and doc://com.apple.documentation/documentation/swiftui/anyview/fullscreencover(item:ondismiss:content:) modifiers in the same view hierarchy. (74246633)

- Dynamic properties such as State, Environment, and others now work correctly in ButtonStyle instances. (62886135)

- ProgressView instances initialized with a Progress object now correctly track updates to the `Progress` object from background threads, and no longer issue a “not allowed” console warning. (69999449)

- InlinePickerStyle now resolves as an in-line section if applied to a Picker within a List on iOS, watchOS, and tvOS, using a checkmark to indicate the selected option. (71383311)

- AppStorage property wrappers now work as expected when contained inside an ObservableObject, causing the system to emit the doc://com.apple.documentation/documentation/combine/observableobject/objectwillchange-2oa5v publisher. (65562845)

- Using scrollTo(_:anchor:) without specifying an anchor now scrolls the List the minimum amount to make it visible. (70184639)

### UIKit

#### Resolved Issues

- leadingAccessoryView and trailingAccessoryView in UITabBar now appear correctly with right-to-left languages. (66755869)

- In a UICollectionView, the focusability of a cell no longer depends on the delegate returning `YES` from the collectionView(_:shouldHighlightItemAt:) and collectionView(_:shouldSelectItemAt:) methods if they are implemented and collectionView(_:canFocusItemAt:) method is not implemented. (70245159)

### Xcode

#### Resolved Issues

- The View Debugger no longer crashes when viewing an app that includes custom Shapes. (72300793)

## See Also

### tvOS 14

tvOS 14.7 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 14.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 14.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 14.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 14.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 14 Release Notes

Update your apps to use new features, and test your apps against API changes.

