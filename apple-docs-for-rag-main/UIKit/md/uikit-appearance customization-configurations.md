

- UIKit
- Appearance customization
-  Configurations 

API Collection

# Configurations

Specify the appearance and content of your views and cells using configurations.

## Overview

Configurations provide a lightweight way to apply content and styling to views without having to manage the rendering of the appearance yourself.

Using a configuration, you can obtain system default styling for a variety of different view states and customize that styling as needed. Then, you assign that configuration to a view that supports configurations, like UICollectionViewCell, or use it to create a custom content view, like UIListContentView. The configuration updates itself when the view’s configuration state changes, causing the view to reflect the new styling for that state.

There are two types of configurations:

- Background configurations, which let you specify background appearance for a view. For more information, see `UIBackgroundConfiguration`.

- Content configurations, which let you specify content (like image and text) and styling for that content (like tint color and padding). For list-based content, UIListContentConfiguration defines many customization options.

## Topics

### Configuration states

struct UIViewConfigurationState

A structure that encapsulates a view’s state.

struct UICellConfigurationState

A structure that encapsulates a cell’s state.

protocol UIConfigurationState

The requirements for an object that encapsulates a view’s state.

struct UIConfigurationStateCustomKey

A key that defines a custom state for a view.

### Content configurations

struct UIListContentConfiguration

A content configuration for a list-based content view.

class UIListContentView

A content view for displaying list-based content.

protocol UIContentConfiguration

The requirements for an object that provides the configuration for a content view.

protocol UIContentView

The requirements for a content view that you create using a configuration.

### Unavailable content configurations

struct UIContentUnavailableConfiguration

A content configuration for a content-unavailable view.

struct UIContentUnavailableConfigurationState

A structure that encapsulates state for a content-unavailable view.

### Background configurations

struct UIBackgroundConfiguration

A configuration that describes a specific background appearance.

### Color transformers

struct UIConfigurationColorTransformer

A transformer that generates a modified output color from an input color.

## See Also

### Appearance and content

Automatic trait tracking

Reduce the need to manually register for trait changes when you use traits within a method or closure that supports automatic trait tracking.

