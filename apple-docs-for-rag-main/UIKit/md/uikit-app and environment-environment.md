

- UIKit
-  App and environment 

API Collection

# App and environment

Manage life-cycle events and your app’s UI scenes, and get information about traits and the environment in which your app runs.

## Overview

In iOS 13 and later, a person can create and manage multiple instances of your app’s user interface simultaneously, and switch between them using the app switcher. On iPad, a person can also display multiple instances of your app side by side. Each instance of your UI displays different content, or displays the same content in a different way. For example, a person can display one instance of the Calendar app showing a specific day, and another showing an entire month.

UIKit communicates details about the current environment using *trait collections*, which reflect a combination of device settings, interface settings, and user preferences. For example, you use traits to detect whether Dark Mode is active for the current view or view controller. Consult the current trait collection of your UIView or UIViewController object when you want to customize its contents based on the current environment. Adopt the UITraitEnvironment protocol in other objects when you want them to receive trait notification changes.

## Topics

### Life cycle

Managing your app’s life cycle

Respond to system notifications when your app is in the foreground or background, and handle other significant system-related events.

Responding to the launch of your app

Initialize your app’s data structures, prepare your app to run, and respond to any launch-time requests from the system.

class UIApplication

The centralized point of control and coordination for apps running in iOS.

protocol UIApplicationDelegate

A set of methods to manage shared behaviors for your app.

Scenes

Manage multiple instances of your app’s UI simultaneously, and direct resources to the appropriate instance of your UI.

### Device environment

class UIDevice

A representation of the current device.

class UIStatusBarManager

An object that describes the configuration of the status bar.

### Adaptivity

Automatic trait tracking

Reduce the need to manually register for trait changes when you use traits within a method or closure that supports automatic trait tracking.

Responding to changing display modes on Apple TV

Change images and resources dynamically when the screen gamut on your device changes.

class UITraitCollection

A collection of data that represents the environment for an individual element in your app’s user interface.

protocol UITraitEnvironment

A set of methods that makes the iOS interface environment available to your app.

protocol UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

protocol UIMutableTraits

A mutable container of traits.

protocol UIAdaptivePresentationControllerDelegate

A set of methods that, in conjunction with a presentation controller, determine how to respond to trait changes in your app.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

### Custom traits

protocol UIMutableTraits

A mutable container of traits.

typealias UITrait

A type representing a trait in a trait collection.

protocol UITraitDefinition

A type representing a trait in a trait collection.

### iPad

Building a desktop-class iPad app

Optimize your iPad app’s user experience by adopting desktop-class enhancements for multitasking with Stage Manager, document interactions, text editing, search, and more.

Elevating your iPad app with a tab bar and sidebar

Provide a compact, ergonomic tab bar for quick access to key parts of your app, and a sidebar for in-depth navigation.

Supporting desktop-class features in your iPad app

Enhance your iPad app by adding desktop-class features and document support.

Multitasking on iPad

Implement multitasking APIs to seamlessly integrate your app with iPadOS.

### Guided Access

protocol UIGuidedAccessRestrictionDelegate

A set of methods you use to add custom restrictions for the Guided Access feature in iOS.

static func guidedAccessRestrictionState(forIdentifier: String) -> UIAccessibility.GuidedAccessRestrictionState

Returns the restriction state for the specified guided access restriction.

### Architecture

Updating your app from 32-bit to 64-bit architecture

Ensure that your app behaves as expected by adapting it to support later versions of the operating system.

func UIApplicationMain(Int32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>, String?, String?) -> Int32

Creates the application object and the application delegate and sets up the event cycle.

## See Also

### App structure

Documents, data, and pasteboard

Organize your app’s data and share that data on the pasteboard.

Resource management

Manage the images, strings, storyboards, and nib files that you use to implement your app’s interface.

App extensions

Extend your app’s basic functionality to other parts of the system.

Interprocess communication

Display activity-based services to people.

Mac Catalyst

Create a version of your iPad app that users can run on a Mac device.

