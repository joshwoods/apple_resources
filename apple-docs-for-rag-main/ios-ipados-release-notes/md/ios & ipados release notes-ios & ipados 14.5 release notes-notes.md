

- iOS &amp; iPadOS Release Notes
-  iOS & iPadOS 14.5 Release Notes 

Article

# iOS & iPadOS 14.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The iOS & iPadOS 14.5 SDK provides support to develop apps for iPhone, iPad, and iPod touch devices running iOS & iPadOS 14.5. The SDK comes bundled with Xcode 12.5, available from the Mac App Store. For information on the compatibility requirements for Xcode 12.5, see Xcode 12.5 Release Notes.

### Accessibility

#### New Features

- Many SF Symbols now have default accessibility labels. (70305995)

### Battery Health

#### Resolved Issues

- iPhone 11, iPhone 11 Pro, and iPhone 11 Pro Max battery health reporting system will recalibrate maximum battery capacity and peak performance capability to address inaccurate estimates of battery health reporting for some users. For more information, see About recalibration of battery health reporting in iOS 14.5.

### Combine

#### Resolved Issues

- Using Published in a subclass of a type conforming to ObservableObject now correctly publishes changes. (71816443)

### Display

#### Resolved Issues

- iOS & iPadOS 14.5 includes an optimization to reduce the appearance of a dim glow that might appear at reduced brightness levels with black backgrounds.

### Privacy

#### New Features

- iPad (8th generation), iPad Air (4th generation), iPad Pro 11-inch (2nd generation), and iPad Pro 12.9-inch (4th generation) now mute the built-in microphone when its Smart Folio is closed. To avoid unnecessarily recording the muted signal, the default behavior is to interrupt an audio session that is using the built-in microphone when the Smart Folio is closed. You can opt out of the playback interruption when the Smart Folio is closed by using the new AVAudioSession.CategoryOptions overrideMutedMicrophoneInterruption, allowing the audio session to continue playing uninterrupted while microphone input remains muted. For more information, see Responding to Audio Session Interruptions. (57042856)

### Siri

#### New Features

- For Music, Podcasts, and Audiobooks requests, updated dialogs for app selection are now available. To ensure your app is set up to participate in Siri app selection, see Improving Siri Media Interactions and App Selection. (74555773)

### SKAdNetwork

#### New Features

- With view-through attribution, SKAdNetwork now supports all ad formats for promoting apps. (70345857)

#### Resolved Issues

- You’re now able to use either version 1.0 or version 2.0 signatures when generated using iOS & iPadOS 14.5 and later. (71474331)

### SwiftUI

#### New Features

- Added TitleAndIconLabelStyle, a new style for Label views that shows both the title and icon of the label using a system-standard layout. In most cases, labels show both title and icon by default. However, some containers might apply a different default label style to their content, such as only showing icons within toolbars on macOS and iOS. To opt in to showing both the title and the icon, apply the title and icon label style: `Label("Lightning", systemImage: "bolt.fill").labelStyle(TitleAndIconLabelStyle())`. (64646578)

- Types conforming to any style protocol, such as ButtonStyle or ToggleStyle, are now enforced to be value types. Styles must be structures or enumerations, not classes, and conforming a class to a style protocol may trigger an assertion. This is the same restriction that the system has always enforced on types conforming to View. (62886135)

#### Resolved Issues

- You can now apply multiple doc://com.apple.documentation/documentation/swiftui/anyview/sheet(ispresented:ondismiss:content:) and doc://com.apple.documentation/documentation/swiftui/anyview/fullscreencover(item:ondismiss:content:) modifiers in the same view hierarchy. (74246633)

- Drop locations are now accurate when using onDrop(of:delegate:). (74030674)

- The doc://com.apple.documentation/documentation/swiftui/ellipse/keyboardshortcut(\_:)-1xmih modifier now works in UIKit lifecycle apps. (73792634)

- Changes to pages that you provide to a TabView with PageTabViewStyle are now correctly reflected in the view. (65701336)

- The dismissal animation of a popover modifier when running in a compact horizontal size class now renders as expected. (52606403)

- Setting doc://com.apple.documentation/documentation/swiftui/text/preferredcolorscheme(\_:) to `nil` now correctly resets to the system’s preferred color scheme. (67000774)

- NavigationView push and pop now correctly respects disabled animations. (70062477)

- HoverEffect no longer causes a ghosting effect, especially over Text. (71344349)

- Using the pointer on iPadOS no longer confuses certain gestures. (71344436)

- onHover(perform:) is now recognized as expected in a stack. (71344436)

- The destination of NavigationLink that only differs by local state now resets that state when switching between links as expected. (72117345)

- Dynamic properties such as State, Environment, and others now work correctly in ButtonStyle instances. (62886135)

- AppStorage property wrappers now work as expected when contained inside an ObservableObject, causing the system to emit the doc://com.apple.documentation/documentation/combine/observableobject/objectwillchange-2oa5v publisher. (65562845)

- ProgressView instances initialized with a Progress object now correctly track updates to the `Progress` object from background threads, and no longer issue a “not allowed” console warning. (69999449)

- Using scrollTo(_:anchor:) without specifying an anchor now scrolls the List the minimum amount to make it visible. (70184639)

- A TabView with PageTabViewStyle now correctly invokes doc://com.apple.documentation/documentation/swiftui/anyview/onappear(perform:) and doc://com.apple.documentation/documentation/swiftui/anyview/ondisappear(perform:) for its tabs. (71225006)

- InlinePickerStyle now resolves as an in-line section if applied to a Picker within a List on iOS, watchOS, and tvOS, using a checkmark to indicate the selected option. (71383311)

### WebKit

#### New Features

- Apps and websites can now receive privacy-preserving attributions for ad clicks which navigate users to websites. (70502338)

### Xcode

#### Deprecations

- Don’t use the iOS MinimumOSVersion information property list key to declare the minimum release of macOS in which your app runs. Use LSMinimumSystemVersion instead. (73890473)

  - Future releases of macOS ignore the `MinimumOSVersion` key in Mac apps, including apps built with Mac Catalyst.

  - Future releases of macOS use the `LSMinimumSystemVersion` key in iOS apps built with Xcode 12.5 or later. If an iOS app doesn’t include an `LSMinimumSystemVersion` key, future releases of macOS compare the app’s `MinimumOSVersion` with the version of its Mac Catalyst runtime to determine compatibility.

## See Also

### iOS &amp; iPadOS 14

iOS & iPadOS 14.7 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.5.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14 Release Notes

Update your apps to use new features, and test your apps against API changes.

