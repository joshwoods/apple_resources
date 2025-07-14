

- macOS Release Notes
-  macOS Big Sur 11.1 Release Notes 

Article

# macOS Big Sur 11.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The macOS 11.1 SDK provides support to develop apps for Macs running macOS Big Sur 11.1. The SDK comes bundled with Xcode 12.3, available from the Mac App Store. For information on the compatibility requirements for Xcode 12.3, see Xcode 12.3 Release Notes.

### AppKit

#### Resolved Issues

- NSToolbar controls now draw the background correctly when you click or roll over them. (71592628)

### Mac Catalyst

#### New Features

- iOS & iPadOS apps with non-resizable windows can now enter full-screen mode. (70103920)

#### Known Issues

- When you present a view controller with page sheet or form sheet presentation style, the size of the view controller’s root view is, by default, determined by the value returned from the presented view controller’s preferredContentSize method and the view is not resizable. You can arrange for the presented view controller to be resizable by using Auto Layout to specify the maximum and minimum sizes of its root view. To enable this, set the canResizeToFitContent property of the application’s main window to YES. One way to do this is to override the willMove(toWindow:) or didMoveToWindow() methods of a view in the main view controller. (65254666)

  For example:

  ```
  - (void)willMoveToWindow:(UIWindow *)newWindow {
      [super willMoveToWindow:newWindow];
      newWindow.canResizeToFitContent = YES;
  }
  ```

## See Also

### macOS 11

macOS Big Sur 11.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Big Sur 11.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Big Sur 11.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Big Sur 11.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Big Sur 11.0.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Big Sur 11.0.1 Universal Apps Release Notes

Update your apps to support Macs with Apple silicon.

macOS Big Sur 11.0.1 iOS & iPadOS Apps on Mac Release Notes

Considerations for running iPhone and iPad apps on Macs with Apple silicon.

