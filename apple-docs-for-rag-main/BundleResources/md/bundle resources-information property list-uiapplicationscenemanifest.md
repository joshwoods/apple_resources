

- Bundle Resources
- Information Property List
-  UIApplicationSceneManifest 

Property List Key

# UIApplicationSceneManifest

The information about the app’s scene-based life-cycle support.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+visionOS 1.0+

## Details 

Name  
Application Scene Manifest

Type  

object

## Discussion

The presence of this key indicates that the app supports scenes and doesn’t use an app delegate object to manage transitions to and from the foreground or background.

## Topics

### Multiple windows

UIApplicationSupportsMultipleScenes

A Boolean value indicating whether the app supports two or more scenes simultaneously.

**Name:** Enable Multiple Windows

UIApplicationSupportsTabbedSceneCollection

A Boolean value indicating whether an app built with Mac Catalyst supports automatic tabbing mode.

**Name:** Supports Tabbed Scene Collection

### CarPlay

CPSupportsDashboardNavigationScene

A Boolean value that indicates whether your app supports displaying navigation content in the CarPlay Dashboard.

CPSupportsInstrumentClusterNavigationScene

A Boolean value that indicates whether your app supports displaying navigation content in the CarPlay Instrument Cluster.

### Configuration

UISceneConfigurations

The default configuration details the system uses to create new scenes.

**Name:** Scene Configuration

## See Also

### Main user interface

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

