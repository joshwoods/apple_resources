

- UIKit
-  UIContentView 

Protocol

# UIContentView

The requirements for a content view that you create using a configuration.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor
protocol UIContentView : NSObjectProtocol
```

## Overview

This protocol provides a blueprint for a content view object that renders the content and styling that you define with its configuration. The content view’s configuration encapsulates all of the supported properties and behaviors for content view customization. Setting the content view’s configuration property applies the new configuration to the view, causing the view to render any updates to its appearance.

## Topics

### Managing the content configuration

var configuration: any UIContentConfiguration

The current configuration of the view.

**Required**

### Determining configuration support

func supports(any UIContentConfiguration) -> Bool

Determines whether the view is compatible with the provided configuration.

**Required** Default implementation provided.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIContentUnavailableView
- UIListContentView

## See Also

### Content configurations

struct UIListContentConfiguration

A content configuration for a list-based content view.

class UIListContentView

A content view for displaying list-based content.

protocol UIContentConfiguration

The requirements for an object that provides the configuration for a content view.

