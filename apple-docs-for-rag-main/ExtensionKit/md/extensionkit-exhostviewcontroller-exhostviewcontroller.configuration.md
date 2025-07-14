

- ExtensionKit
- EXHostViewController
-  EXHostViewController.Configuration 

Structure

# EXHostViewController.Configuration

An object that holds configuration options for a host view controller.

macOS 13.0+

``` source
struct Configuration
```

## Topics

### Creating a Configuration Object

init(appExtension: AppExtensionIdentity, sceneID: String)

Creates a new configuration object.

### Identifying the Extension

var appExtension: AppExtensionIdentity

The app extension for this configuration object.

var sceneID: String

The unique identifier for this configuration object’s user interface.

## See Also

### Configuring the View Controller

var configuration: EXHostViewController.Configuration?

The view controller’s configuration.

var placeholderView: NSView

A view that’s used when the view controller has no content to display.

