

- UIKit
-  UIConfigurationState 

Protocol

# UIConfigurationState

The requirements for an object that encapsulates a view’s state.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
protocol UIConfigurationState
```

## Overview

This protocol provides a blueprint for a configuration state object, which encompasses a trait collection along with all of the common states that affect a view’s appearance. A configuration state encapsulates the inputs that configure a view for any possible state or combination of states. You use a configuration state with background and content configurations to obtain the default appearance for a specific state.

Typically, you don’t create a configuration state yourself. To obtain a configuration state, override the updateConfiguration(using:) method in your view subclass and use the state parameter. Outside of this method, you can get a view’s configuration state by using its configurationState property.

For more information, see UIViewConfigurationState and UICellConfigurationState.

## Topics

### Managing configuration states

var traitCollection: UITraitCollection

The traits that describe the current layout environment of the view, such as the user interface style and layout direction.

**Required**

subscript(UIConfigurationStateCustomKey) -> AnyHashable?

Accesses custom states by key.

**Required**

### Creating a configuration state manually

init(traitCollection: UITraitCollection)

Creates a view configuration state with the specified trait collection.

**Required**

## Relationships

### Conforming Types

- UICellConfigurationState
- UIContentUnavailableConfigurationState
- UIViewConfigurationState

## See Also

### Configuration states

struct UIViewConfigurationState

A structure that encapsulates a view’s state.

struct UICellConfigurationState

A structure that encapsulates a cell’s state.

struct UIConfigurationStateCustomKey

A key that defines a custom state for a view.

