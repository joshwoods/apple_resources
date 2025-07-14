

- UIKit
-  UIActivityItemsConfigurationInteraction 

Structure

# UIActivityItemsConfigurationInteraction

A structure that describes types of interactions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct UIActivityItemsConfigurationInteraction
```

## Overview

Specify which interactions you want the activity view to include in supportedInteractions.

## Topics

### Selecting interactions

static let copy: UIActivityItemsConfigurationInteraction

The copy interaction.

static let share: UIActivityItemsConfigurationInteraction

The share interaction.

### Creating an interaction type

init(String)

Creates an activity items configuration interaction.

init(rawValue: String)

Creates an activity items configuration interaction with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing supported interactions

var supportedInteractions: [UIActivityItemsConfigurationInteraction]

The types of interactions that the configuration supports.

