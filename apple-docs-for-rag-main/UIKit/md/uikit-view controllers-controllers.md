

- UIKit
-  View controllers 

API Collection

# View controllers

Manage your interface using view controllers and facilitate navigation around your app’s content.

## Overview

You use view controllers to manage your UIKit app’s interface. A view controller manages a single root view, which may itself contain any number of subviews. User interactions with that view hierarchy are handled by your view controller, which coordinates with other objects of your app as needed. Every app has at least one view controller whose content fills the main window. If your app has more content than can fit onscreen at once, use multiple view controllers to manage different parts of that content.

A *container view controller* embeds the content of other view controllers into its own root view. A container view controller may mix custom views with the contents of its child view controllers to facilitate navigation or to create unique interfaces. For example, a UINavigationController object manages a navigation bar and a stack of child view controllers (only one of which is visible at a time), and provides an API to add and remove child view controllers from the stack.

UIKit provides several standard view controllers for navigation and managing specific types of content. You define the view controllers containing your app’s custom content. You may also define custom container view controllers to implement new navigation schemes.

## Topics

### Essentials

Managing content in your app’s windows

Build your app’s user interface from view controllers, and change the currently visible view controller when you want to display new content.

UIKit Catalog: Creating and customizing views and controls

Customize your app’s user interface with views and controls.

### Content view controllers

Displaying and managing views with a view controller

Build a view controller in storyboards, configure it with custom views, and fill those views with your app’s data.

Showing and hiding view controllers

Display view controllers using different techniques, and pass data between them during transitions.

class UIViewController

An object that manages a view hierarchy for your UIKit app.

class UITableViewController

A view controller that specializes in managing a table view.

class UICollectionViewController

A view controller that specializes in managing a collection view.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

### Container view controllers

Creating a custom container view controller

Create a composite interface by combining content from one or more view controllers with other custom views.

class UISplitViewController

A container view controller that implements a hierarchical interface.

class UINavigationController

A container view controller that defines a stack-based scheme for navigating hierarchical content.

class UINavigationBar

Navigational controls that display in a bar along the top of the screen, usually in conjunction with a navigation controller.

class UINavigationItem

The items that a navigation bar displays when the associated view controller is visible.

class UITabBarController

A container view controller that manages a multiselection interface, where the selection determines which child view controller to display.

class UITabBar

A control that displays one or more buttons in a tab bar for selecting between different subtasks, views, or modes in an app.

class UITabBarItem

An object that describes an item in a tab bar.

class UITab

An object that manages a tab in a tab bar.

class UISearchTab

A tab subclass that represents the system’s search tab.

class UITabGroup

An object that manages a collection of tab objects.

class UIPageViewController

A container view controller that manages navigation between pages of content, where a subview controller manages each page.

### Presentation management

Disabling the pull-down gesture for a sheet

Ensure a positive user experience when presenting a view controller as a sheet.

class UIPresentationController

An object that manages the transition animations and the presentation of view controllers onscreen.

class UISheetPresentationController

A presentation controller that manages the appearance and behavior of a sheet.

### Search interface

class UISearchContainerViewController

A view controller that manages the presentation of search results in your interface.

class UISearchController

A view controller that manages the display of search results based on interactions with a search bar.

class UISearchBar

A specialized view for receiving search-related information from the user.

protocol UISearchResultsUpdating

A set of methods that let you update search results based on information the user enters into the search bar.

Displaying searchable content by using a search controller

Create a user interface with searchable content in a table view.

Using suggested searches with a search controller

Create a search interface with a table view of suggested searches.

### Images and video

class UIImagePickerController

A view controller that manages the system interfaces for taking pictures, recording movies, and choosing items from the user’s media library.

class UIVideoEditorController

A view controller that manages the system interface for trimming video frames and encoding a previously recorded movie.

### Documents and directories

Customizing a document-based app’s launch experience

Add unique elements to your app’s document launch scene.

Adding a document browser to your app

Give users access to their local or remote documents from within your app.

Providing access to directories

Use a document picker to access the content of a directory outside your app’s container.

Building a document browser-based app

Use a document browser to provide access to the user’s text files.

Building a document browser app for custom file formats

Implement a custom document file format to manage user interactions with files on different cloud storage providers.

class UIDocumentViewController

A view controller that manages and presents a document stored locally or in the cloud.

class UIDocumentBrowserViewController

A view controller for browsing and performing actions on documents that you store locally and in the cloud.

class UIDocumentPickerViewController

A view controller that provides access to documents or destinations outside your app’s sandbox.

class UIDocumentInteractionController

A view controller that previews, opens, or prints files with a file format that your app can’t handle directly.

### iCloud Sharing

class UICloudSharingController

A view controller that presents standard screens for adding and removing people from a CloudKit share record.

### Activities interface

Collaborating and sharing copies of your data

Share data and collaborate with people from your app.

class UIActivityViewController

A view controller that you use to offer standard services from your app.

class UIActivityItemProvider

A proxy for data that passes to an activity view controller.

protocol UIActivityItemSource

A set of methods that an activity view controller uses to retrieve the data items to act on.

class UIActivity

An abstract class that you subclass to implement app-specific services.

protocol UIActivityItemsConfigurationProviding

An interface that provides a source for shareable content to fulfill user requests to share current content.

### Font picker

class UIFontPickerViewController

A view controller that manages the interface for selecting a font that the system provides or the user installs.

protocol UIFontPickerViewControllerDelegate

A set of optional methods for receiving messages about the user’s interaction with the font picker.

class Configuration

The filters and display settings a font picker view controller uses to set up a font picker.

### Color picker

class UIColorPickerViewController

A view controller that manages the interface for selecting a color.

protocol UIColorPickerViewControllerDelegate

The delegate protocol to inform about changes in color selection.

### Word lookup

class UIReferenceLibraryViewController

A view controller that displays a standard interface for looking up the definition of a word or term.

### Printer picker

class UIPrinterPickerController

A view controller that displays the standard interface for selecting a printer.

### Interface orientation

var isPortrait: Bool

A Boolean value that indicates whether the user interface is currently presented in a portrait orientation.

var isLandscape: Bool

A Boolean value that indicates whether the user interface is currently presented in a landscape orientation.

### Interface restoration

Restoring your app’s state

Provide continuity for the user by preserving current activities.

Restoring Your App’s State with SwiftUI

Provide app continuity for users by preserving their current activities.

Preserving your app’s UI across launches

Return your app to its previous state after the system terminates it.

protocol UIViewControllerRestoration

The methods that objects adopt so that they can act as a restoration class for view controllers during state restoration.

protocol UIObjectRestoration

The interface that restoration classes use to restore preserved objects.

protocol UIStateRestoring

Methods for adding objects to your state restoration archives.

## See Also

### User interface

Views and controls

Present your content onscreen and define the interactions allowed with that content.

View layout

Use stack views to lay out the views of your interface automatically. Use Auto Layout when you require precise placement of your views.

Appearance customization

Add Dark Mode support to your app, customize the appearance of bars, and use appearance proxies to modify your UI.

Animation and haptics

Provide feedback to users using view-based animations and haptics.

Windows and screens

Provide a container for your view hierarchies and other content.

