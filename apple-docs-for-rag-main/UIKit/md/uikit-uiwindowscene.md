

- UIKit
-  UIWindowScene 

Class

# UIWindowScene

A scene that manages one or more windows for your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIWindowScene
```

## Mentioned in 

Specifying the scenes your app supports

Presenting content on a connected display

## Overview

A UIWindowScene object manages one instance of your app’s UI, including one or more windows that you display from that scene. The scene object manages the display of your windows on the user’s device, and the life cycle of that scene as the user interacts with it. When the state of the scene changes, the scene object notifies its delegate object, which adopts the UIWindowSceneDelegate protocol. The scene also posts appropriate notifications to registered observers. Use the delegate object or notification observers to respond to any changes.

Don’t create window scene objects directly. Instead, specify that you want a UIWindowScene object at configuration time by including the class name for the scene in the scene configuration details of your app’s `Info.plist` file. You can also specify the class name when creating a UISceneConfiguration object in your app delegate’s application(_:configurationForConnecting:options:) method. When the user interacts with your app, the system creates an appropriate scene object based on the configuration data you provided. To create a scene programmatically, call the requestSceneSessionActivation(_:userActivity:options:errorHandler:) method of UIApplication.

## Topics

### Getting the active windows

var windows: [UIWindow]

The windows associated with the scene.

var keyWindow: UIWindow?

The key window associated with the scene.

var screen: UIScreen

The screen that displays the contents of the scene.

### Getting the interface attributes

var traitCollection: UITraitCollection

The traits that describe the current environment of the scene.

var coordinateSpace: any UICoordinateSpace

The coordinate space occupied by the scene.

var interfaceOrientation: UIInterfaceOrientation

The orientation to use when displaying content in your windows.

var sizeRestrictions: UISceneSizeRestrictions?

The minimum and maximum size of the app’s windows.

class UISceneSizeRestrictions

An object that specifies the minimum and maximum sizes for resizable windows.

### Observing trait changes

protocol UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

### Overriding trait values

var traitOverrides: UITraitOverrides

struct UITraitOverrides

### Providing a PDF version of your scene

var screenshotService: UIScreenshotService?

An object that generates a high-fidelity version of your app’s content.

class UIScreenshotService

An object that coordinates the creation of PDF screenshots of an app’s content.

### Sharing content

var activityItemsConfigurationSource: (any UIActivityItemsConfigurationProviding)?

An object that can provide shareable items for a scene.

protocol UIActivityItemsConfigurationProviding

An interface that provides a source for shareable content to fulfill user requests to share current content.

### Determining window behaviors

var isFullScreen: Bool

A Boolean value that indicates whether the window scene is full screen or windowed.

var windowingBehaviors: UISceneWindowingBehaviors?

An object that specifies the behaviors of the window.

class UISceneWindowingBehaviors

An object with properties that determine the behavior of a window.

### Working with window geometry

var effectiveGeometry: UIWindowScene.Geometry

The current values for the window scene’s geometry in system space.

func requestGeometryUpdate(UIWindowScene.GeometryPreferences, errorHandler: ((any Error) -> Void)?)

Requests an update to the window scene’s geometry using the specified geometry preferences object.

class Geometry

An object that provides geometry information about the window scene.

class GeometryPreferences

An abstract superclass for representing window scene geometry preferences.

class iOS

An object that represents the geometry preferences for a window scene in an iOS app.

class Mac

An object that represents the geometry preferences for a window scene in an app built with Mac Catalyst.

class Vision

let UIProposedSceneSizeNoPreference: CGFloat

### Working with focus

var focusSystem: UIFocusSystem?

The focus system that’s responsible for the window scene.

### Getting the status bar configuration

var statusBarManager: UIStatusBarManager?

The current configuration of the status bar.

class UIStatusBarManager

An object that describes the configuration of the status bar.

### Configuring a window’s title bar

var titlebar: UITitlebar?

The title bar displayed in a window of a Mac app.

class UITitlebar

An object that you use to configure the title bar of a window in a Mac app built with Mac Catalyst.

### Supporting types

class ActivationAction

A menu element that requests a window scene.

class ActivationConfiguration

An object that provides configuration options for a window scene request.

class ActivationInteraction

An interaction that facilitates activating a window scene when a user pinches out on the interaction’s view.

class ActivationRequestOptions

An object that contains information you want the system to use when activating a new window scene.

class UIWindowSceneDestructionRequestOptions

An object that contains information to use when removing a window scene from your app.

enum DismissalAnimation

Constants that indicate the types of animations available for dismissing a scene’s windows.

class UIWindowSceneDragInteraction

An interaction you add to a view that enables pan gestures to change the containing window scene’s position.

enum ResizingRestrictions

enum UIWindowSceneResizingRestrictions

enum PresentationStyle

The placement of a window scene relative to other scenes in the workspace.

Deprecated

## Relationships

### Inherits From

- UIScene

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Window scenes

Supporting multiple windows on iPad

Support side-by-side instances of your app’s interface and create new windows.

protocol UIWindowSceneDelegate

Additional methods that you use to manage app-specific tasks occurring in a scene.

class UIScene

An object that represents one instance of your app’s user interface.

protocol UISceneDelegate

The core methods you use to respond to life-cycle events occurring within a scene.

