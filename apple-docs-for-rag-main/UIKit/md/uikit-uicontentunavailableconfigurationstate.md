

- UIKit
-  UIContentUnavailableConfigurationState 

Structure

# UIContentUnavailableConfigurationState

A structure that encapsulates state for a content-unavailable view.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
struct UIContentUnavailableConfigurationState
```

## Overview

Typically, you don’t create a configuration state yourself. To obtain a configuration state, override updateContentUnavailableConfiguration(using:) in your view controller subclass and use the state parameter. Outside of this method, you can get a view controller’s configuration state from the contentUnavailableConfigurationState property.

You can create your own custom states to add to a content-unavailable configuration state by defining a custom state key with UIConfigurationStateCustomKey.

## Topics

### Instance Properties

var searchText: String?

The search text.

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

### Unavailable content configurations

struct UIContentUnavailableConfiguration

A content configuration for a content-unavailable view.

