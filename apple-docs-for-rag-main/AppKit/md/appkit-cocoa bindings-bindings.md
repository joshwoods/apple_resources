

- AppKit
-  Cocoa Bindings 

API Collection

# Cocoa Bindings

Automatically synchronize your data model with your app’s interface using Cocoa Bindings.

## Topics

### Core Controllers

class NSObjectController

A controller that can manage an object’s properties referenced by key-value paths.

class NSController

An abstract class that implements the NSEditor and NSEditorRegistration informal protocols required for controller classes.

### Tree-Based Data

Navigating Hierarchical Data Using Outline and Split Views

Build a structured user interface that simplifies navigation in your app.

class NSTreeController

A bindings-compatible controller that manages a tree of objects.

class NSTreeNode

A node in a tree of nodes.

### Array-Based Data

class NSArrayController

A bindings-compatible controller that manages a collection of objects.

### Key-Value Data

class NSDictionaryController

A bindings-compatible controller that manages the display and editing of a dictionary of key-value pairs.

class NSDictionaryControllerKeyValuePair

A set of methods implemented by arranged objects to give access to information about those objects.

struct NSBindingName

Values that specify a binding for certain methods.

struct NSBindingOption

struct NSBindingInfoKey

func NSIsControllerMarker(Any?) -> Bool

Tests whether a given object is special marker object used for indicating the state of a selection in relation to a key.

NSKeyValueBindingCreation

A set of methods that you can use to create and remove bindings between view objects and controllers, or between controllers and model objects.

Binding dictionary keys

These constants define keys in the binding information dictionary.

### Data Placeholders

class NSBindingSelectionMarker

NSPlaceholders

A set of methods that an object can implement to register default placeholders to be displayed for a binding, when no other placeholder is specified.

## See Also

### App Structure

App and Environment

Learn about the objects that you use to interact with the system.

Documents, Data, and Pasteboard

Organize your app’s data and preferences, and share that data on the pasteboard or in iCloud.

Resource Management

Manage the storyboards and nib files containing your app’s user interface, and learn how to load data that is stored in resource files.

App Extensions

Extend your app’s basic functionality to other parts of the system.

