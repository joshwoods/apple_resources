

- UIKit
-  UIContentConfiguration 

Protocol

# UIContentConfiguration

The requirements for an object that provides the configuration for a content view.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
protocol UIContentConfiguration
```

## Overview

This protocol provides a blueprint for a content-configuration object, which encompasses default styling and content for a content view. The content configuration encapsulates all of the supported properties and behaviors for content view customization. You use the configuration to create the content view.

## Topics

### Creating a content configuration

func makeContentView() -> any UIView &amp; UIContentView

Creates a new instance of the content view using this configuration.

**Required**

### Updating a content configuration

func updated(for: any UIConfigurationState) -> Self

Generates a configuration for the specified state by applying the configuration’s default values for that state to any properties that you haven’t customized.

**Required**

## Relationships

### Conforming Types

- UIContentUnavailableConfiguration
- UIListContentConfiguration

## See Also

### Content configurations

struct UIListContentConfiguration

A content configuration for a list-based content view.

class UIListContentView

A content view for displaying list-based content.

protocol UIContentView

The requirements for a content view that you create using a configuration.

