

- UIKit
-  UIStoryboard 

Class

# UIStoryboard

An encapsulation of the design-time view controller graph represented in an Interface Builder storyboard resource file.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
class UIStoryboard
```

## Mentioned in 

Displaying and managing views with a view controller

## Overview

A UIStoryboard object manages archived versions of your app’s view controllers. At design time, you configure the content of your view controllers visually, and Xcode saves the data needed to recreate that interface in a storyboard file in your app’s bundle. When you want to create a new view controller programmatically, first create a UIStoryboard object and specify the appropriate name and bundle information. Then use that object to instantiate the specific view controller that you want.

During the instantiation process, UIStoryboard creates your view controller programmatically using its init(coder:) method. The storyboard passes the view controller’s data archive to that method, which then uses the data to recreate the state of the view controller and its views. If you have a custom initialization method for your view controller, you can ask the storyboard to instantiate your view controller using a block you provide. You can use this block to call your custom initialization method, passing any extra data your view controller needs.

For visionOS apps, you can load existing storyboards, but you can’t add content specific to the platform. Migrate your interface code to SwiftUI as soon as possible.

## Topics

### Getting a Storyboard Object

init(name: String, bundle: Bundle?)

Creates and returns a storyboard object for the specified resource file.

### Loading the Initial View Controller

func instantiateInitialViewController() -> UIViewController?

Creates the initial view controller and initializes it with the data from the storyboard.

func instantiateInitialViewController&lt;ViewController>(creator: ((NSCoder) -> ViewController?)?) -> ViewController?

Creates the initial view controller from the storyboard and initializes it using your custom initialization code.

### Instantiating Storyboard View Controllers

func instantiateViewController(withIdentifier: String) -> UIViewController

Creates the view controller with the specified identifier and initializes it with the data from the storyboard.

func instantiateViewController&lt;ViewController>(identifier: String, creator: ((NSCoder) -> ViewController?)?) -> ViewController

Creates the specified view controller from the storyboard and initializes it using your custom initialization code.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Storyboards

Customizing the behavior of segue-based presentations

Pass data between view controllers during a segue, and programmatically control when segues occur.

Dismissing a view controller with an unwind segue

Configure an unwind segue in your storyboard file that dynamically chooses the most appropriate view controller to display next.

class UIStoryboardSegue

An object that prepares for and performs the visual transition between two view controllers.

class UIStoryboardUnwindSegueSource

An encapsulation of information about an unwind segue.

