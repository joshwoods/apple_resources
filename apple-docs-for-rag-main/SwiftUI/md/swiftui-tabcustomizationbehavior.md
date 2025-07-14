

- SwiftUI
-  TabCustomizationBehavior 

Structure

# TabCustomizationBehavior

The customization behavior of customizable tab view content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TabCustomizationBehavior
```

## Overview

Use this type in conjunction with the customizationBehavior(_:for:) modifier.

## Topics

### Type Properties

static var automatic: TabCustomizationBehavior

The automatic customization behavior.

static var disabled: TabCustomizationBehavior

The customization behavior isn’t available.

static var reorderable: TabCustomizationBehavior

The reorderable customization behavior.

## Relationships

### Conforms To

- Equatable

## See Also

### Enabling tab customization

func tabViewCustomization(Binding&lt;TabViewCustomization>?) -> some View

Specifies the customizations to apply to the sidebar representation of the tab view.

struct TabViewCustomization

The customizations a person makes to an adaptable sidebar tab view.

