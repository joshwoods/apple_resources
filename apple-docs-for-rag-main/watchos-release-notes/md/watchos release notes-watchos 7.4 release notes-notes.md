

- watchOS Release Notes
-  watchOS 7.4 Release Notes 

Article

# watchOS 7.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The watchOS 7.4 SDK provides support to develop watchOS apps for Apple Watch devices running watchOS 7.4. The SDK comes bundled with Xcode 12.5, available from the Mac App Store. For information on the compatibility requirements for Xcode 12.5, see Xcode 12.5 Release Notes.

### Accessibility

#### New Features

- Many SF Symbols now have default accessibility labels. (70305995)

### Combine

#### Resolved Issues

- Using Published in a subclass of a type conforming to ObservableObject now correctly publishes changes. (71816443)

### SwiftUI

#### New Features

- Added TitleAndIconLabelStyle, a new style for Label views that shows both the title and icon of the label using a system-standard layout. In most cases, labels show both title and icon by default. However, some containers might apply a different default label style to their content, such as only showing icons within toolbars on macOS and iOS. To opt in to showing both the title and the icon, apply the title and icon label style: `Label("Lightning", systemImage: "bolt.fill").labelStyle(TitleAndIconLabelStyle())`. (64646578)

- Types conforming to any style protocol, such as ButtonStyle or ToggleStyle, are now enforced to be value types. Styles must be structures or enumerations, not classes, and conforming a class to a style protocol may trigger an assertion. This is the same restriction that the system has always enforced on types conforming to View. (62886135)

#### Resolved Issues

- Dynamic properties such as State, Environment, and others now work correctly in ButtonStyle instances. (62886135)

- ProgressView instances initialized with a Progress object now correctly track updates to the `Progress` object from background threads, and no longer issue a “not allowed” console warning. (69999449)

- InlinePickerStyle now resolves as an in-line section if applied to a Picker within a List on iOS, watchOS, and tvOS, using a checkmark to indicate the selected option. (71383311)

- AppStorage property wrappers now work as expected when contained inside an ObservableObject, causing the system to emit the doc://com.apple.documentation/documentation/combine/observableobject/objectwillchange-2oa5v publisher. (65562845)

- Using scrollTo(_:anchor:) without specifying an anchor now scrolls the List the minimum amount to make it visible. (70184639)

- A TabView with PageTabViewStyle now correctly invokes doc://com.apple.documentation/documentation/swiftui/anyview/onappear(perform:) and doc://com.apple.documentation/documentation/swiftui/anyview/ondisappear(perform:) for its tabs. (71225006)

## See Also

### watchOS 7

watchOS 7.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 7.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 7.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 7.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 7.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 7 Release Notes

Update your apps to use new features, and test your apps against API changes.

