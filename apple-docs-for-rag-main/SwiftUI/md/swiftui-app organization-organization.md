

- SwiftUI
-  App organization 

API Collection

# App organization

Define the entry point and top-level structure of your app.

## Overview

Describe your app’s structure declaratively, much like you declare a view’s appearance. Create a type that conforms to the App protocol and use it to enumerate the Scenes that represent aspects of your app’s user interface.

SwiftUI enables you to write code that works across all of Apple’s platforms. However, it also enables you to tailor your app to the specific capabilities of each platform. For example, if you need to respond to the callbacks that the system traditionally makes on a UIKit, AppKit, or WatchKit app’s delegate, define a delegate object and instantiate it in your app structure using an appropriate delegate adaptor property wrapper, like UIApplicationDelegateAdaptor.

For platform-specific design guidance, see Getting started in the Human Interface Guidelines.

## Topics

### Creating an app

Destination Video

Leverage SwiftUI to build an immersive media experience in a multiplatform app.

Hello World

Use windows, volumes, and immersive spaces to teach people about the Earth.

Backyard Birds: Building an app with SwiftData and widgets

Create an app with persistent data, interactive widgets, and an all new in-app purchase experience.

Food Truck: Building a SwiftUI multiplatform app

Create a single codebase and app target for Mac, iPad, and iPhone.

Fruta: Building a Feature-Rich App with SwiftUI

Create a shared codebase to build a multiplatform app that offers widgets and an App Clip.

Migrating to the SwiftUI life cycle

Use a scene-based life cycle in SwiftUI while keeping your existing codebase.

protocol App

A type that represents the structure and behavior of an app.

### Targeting iOS and iPadOS

UILaunchScreen

The user interface to show while an app launches.

UILaunchScreens

The user interfaces to show while an app launches in response to different URL schemes.

struct UIApplicationDelegateAdaptor

A property wrapper type that you use to create a UIKit app delegate.

### Targeting macOS

struct NSApplicationDelegateAdaptor

A property wrapper type that you use to create an AppKit app delegate.

### Targeting watchOS

struct WKApplicationDelegateAdaptor

A property wrapper that is used in `App` to provide a delegate from WatchKit.

struct WKExtensionDelegateAdaptor

A property wrapper type that you use to create a WatchKit extension delegate.

### Targeting tvOS

Creating a tvOS media catalog app in SwiftUI

Build standard content lockups and rows of content shelves for your tvOS app.

## See Also

### App structure

Scenes

Declare the user interface groupings that make up the parts of your app.

Windows

Display user interface content in a window or a collection of windows.

Immersive spaces

Display unbounded content in a person’s surroundings.

Documents

Enable people to open and manage documents.

Navigation

Enable people to move between different parts of your app’s view hierarchy within a scene.

Modal presentations

Present content in a separate view that offers focused interaction.

Toolbars

Provide immediate access to frequently used commands and controls.

Search

Enable people to search for text or other content within your app.

App extensions

Extend your app’s basic functionality to other parts of the system, like by adding a Widget.

