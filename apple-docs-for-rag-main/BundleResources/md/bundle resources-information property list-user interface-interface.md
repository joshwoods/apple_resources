

- Bundle Resources
- Information Property List
-  User interface 

API Collection

# User interface

Configure an app’s scenes, storyboards, icons, fonts, and other user interface elements.

## Overview

You define the user interface that your app presents during normal operation with a combination of code and storyboards. However, the system needs to know a few things about your app’s user interface before execution begins. For example, on some platforms, you have to specify what device orientations your app supports and what the system should display while your app launches. You add keys to your app’s Information Property List file to control certain aspects of its user interface.

## Topics

### Main user interface

UIApplicationSceneManifest

The information about the app’s scene-based life-cycle support.

**Name:** Application Scene Manifest

UIApplicationPreferredDefaultSceneSessionRole

The preferred initial scene session role for your app.

NSMainStoryboardFile

The name of an app’s storyboard resource file.

**Name:** Main storyboard file base name

UIMainStoryboardFile

The name of the app’s main storyboard file.

**Name:** Main storyboard file base name

NSMainNibFile

The name of an app’s main user interface file.

**Name:** Main nib file base name

LSUIElement

A Boolean value indicating whether the app is an agent app that runs in the background and doesn’t appear in the Dock.

**Name:** Application is agent (UIElement)

UISupportsTrueScreenSizeOnMac

A Boolean value that indicates whether your iPad app supports arbitrary screen sizes and resolutions when running on a Mac.

### Launch interface

UILaunchScreen

The user interface to show while an app launches.

UILaunchScreens

The user interfaces to show while an app launches in response to different URL schemes.

UILaunchStoryboardName

The filename of the storyboard from which to generate the app’s launch image.

**Name:** Launch screen interface file base name

UILaunchStoryboards

The launch storyboard to use to generate a launch image when your app opens from a supported scheme.

LSUIPresentationMode

The initial user-interface mode for the app.

**Name:** Application UI Presentation Mode

UILaunchToFullScreenByDefaultOnMac

A Boolean value that indicates whether to launch your iPad app in full-screen mode when running on a Mac.

### Icons

CFBundleIcons

Information about all of the icons used by the app.

**Name:** Icon files (iOS 5)

CFBundleIconFiles

The names of the bundle’s icon image files.

**Name:** Icon files

CFBundleIconFile

The file containing the bundle’s icon.

**Name:** Icon file

CFBundleIconName

The name of the asset that represents the app icon.

**Name:** Icon Name

UIPrerenderedIcon

A Boolean value that indicates whether the app’s icon contains a shine effect.

**Name:** Icon already includes gloss effects

### Orientation

UIInterfaceOrientation

The initial orientation of the app’s user interface.

**Name:** Initial interface orientation

UISupportedInterfaceOrientations

The interface orientations supported by your app.

**Name:** Supported interface orientations

UIPreferredDefaultInterfaceOrientation

A string that indicates the preferred initial interface orientation for iPad and iPhone apps running on visionOS.

### Styling

UIUserInterfaceStyle

The user interface style for the app.

**Name:** User Interface Style

UIViewEdgeAntialiasing

A Boolean value that indicates whether Core Animation layers use antialiasing when drawing a layer that isn’t aligned to pixel boundaries.

**Name:** Renders with edge antialiasing

UIWhitePointAdaptivityStyle

The app’s white-point adaptivity style, enabled on devices with True Tone displays.

**Name:** White Point Adaptivity Style

UIViewGroupOpacity

A Boolean value that indicates whether Core Animation sublayers inherit the opacity of their superlayer.

**Name:** Renders with group opacity

UIRequiresFullScreen

A Boolean value that indicates whether an iPad app is capable of sharing the screen with other apps.

UISupportsFullScreenInAssistiveAccess

A Boolean value that indicates if an iOS or iPadOS app appears as full screen in Assistive Access.

**Name:** Supports full screen in Assistive Access

NSPrefersDisplaySafeAreaCompatibilityMode

A Boolean value that indicates whether the app prefers to run in compatibility mode when necessary.

NSAccentColorName

The name of a color in an asset catalog to use for a target’s global accent color.

NSWidgetBackgroundColorName

The name of a color in an asset catalog to use for a widget’s configuration interface.

### Fonts

ATSApplicationFontsPath

The location of a font file or folder of fonts in the bundle’s Resources folder.

**Name:** Application fonts resource path

UIAppFonts

App-specific font files located in the bundle and that the system loads at runtime.

**Name:** Fonts provided by application

### Status bar

UIStatusBarHidden

A Boolean value that indicates whether the system initially hides the status bar when the app launches.

**Name:** Status bar is initially hidden

UIStatusBarStyle

The style of the status bar as the app launches.

**Name:** Status bar style

UIStatusBarTintParameters

The status bar tint.

**Name:** Status bar tinting parameters

UIViewControllerBasedStatusBarAppearance

A Boolean value that indicates whether the system bases the appearance of the status bar on the style preferred by the current view controller.

**Name:** View controller-based status bar appearance

### Pointer interactions

UIApplicationSupportsIndirectInputEvents

A Boolean value indicating that the app generally supports indirect input mechanisms.

### Preferences

NSPrefPaneIconFile

The name of an image file used to represent a preference pane in the System Preferences app.

**Name:** Preference Pane icon file

NSPrefPaneIconLabel

The name of a preference pane displayed beneath the preference pane icon in the System Preferences app.

**Name:** Preference Pane icon label

### Graphics

UIAppSupportsHDR

A Boolean value that indicates whether the app supports HDR mode on Apple TV 4K.

**Name:** Supports HDR color mode

NSHighResolutionCapable

A Boolean value indicating whether the Cocoa app supports high-resolution displays.

**Name:** High Resolution Capable

NSSupportsAutomaticGraphicsSwitching

A Boolean value indicating whether an OpenGL app may utilize the integrated GPU.

**Name:** Supports Automatic Graphics Switching

GPUEjectPolicy

The preferred system action when an external GPU is connected from the system.

GPUSelectionPolicy

The app’s preference for whether it wants to use external graphics processors.

### QuickLook

QLNeedsToBeRunInMainThread

A Boolean value indicating whether a Quick Look app’s generator can be run in threads other than the main thread.

**Name:** Quick Look needs to be run in main thread

QLPreviewHeight

A hint at the height, in points, of a Quick Look app’s previews.

**Name:** Quick Look preview height

QLPreviewWidth

A hint at the width, in points, of a Quick Look app’s previews.

**Name:** Quick Look preview width

QLSupportsConcurrentRequests

A Boolean value indicating whether a Quick Look app’s generator can handle concurrent thumbnail and preview requests.

**Name:** Quick Look supports concurrent requests

QLThumbnailMinimumSize

The minimum size, in points, along one dimension of thumbnails for a Quick Look app’s generator.

**Name:** Quick Look thumbnail minimum size

### Deprecated keys

UILaunchImages

A dictionary containing information about launch images.

Deprecated

## See Also

### Core settings

Bundle configuration

Define basic characteristics of a bundle, like its name, type, and version.

App execution

Control app launch, execution, and termination.

