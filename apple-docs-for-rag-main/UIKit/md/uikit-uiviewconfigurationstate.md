

- UIKit
-  UIViewConfigurationState 

Structure

# UIViewConfigurationState

A structure that encapsulates a view’s state.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct UIViewConfigurationState
```

## Overview

A view configuration state encompasses a trait collection along with all of the common states that affect a view’s appearance — states like selected, focused, or disabled. A view configuration state encapsulates the inputs that configure a view for any possible state or combination of states. You use a view configuration state with background and content configurations to obtain the default appearance for a specific state.

Typically, you don’t create a configuration state yourself. To obtain a configuration state, override the updateConfiguration(using:) method in your view subclass and use the state parameter. Outside of this method, you can get a view’s configuration state by using its configurationState property.

You can create your own custom states to add to a view configuration state by defining a custom state key using UIConfigurationStateCustomKey.

## Topics

### Managing view configuration states

var isSelected: Bool

A Boolean value that indicates whether the view is in a selected state.

var isHighlighted: Bool

A Boolean value that indicates whether the view is in a highlighted state.

var isFocused: Bool

A Boolean value that indicates whether the view is in a focused state.

var isDisabled: Bool

A Boolean value that indicates whether the view is in a disabled state.

var isPinned: Bool

A Boolean value that indicates whether the view is in a pinned state.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- UIConfigurationState

## See Also

### Configuration states

struct UICellConfigurationState

A structure that encapsulates a cell’s state.

protocol UIConfigurationState

The requirements for an object that encapsulates a view’s state.

struct UIConfigurationStateCustomKey

A key that defines a custom state for a view.

