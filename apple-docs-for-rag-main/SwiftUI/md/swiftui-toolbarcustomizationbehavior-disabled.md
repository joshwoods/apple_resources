

- SwiftUI
- ToolbarCustomizationBehavior
-  disabled 

Type Property

# disabled

The disabled customization behavior.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var disabled: ToolbarCustomizationBehavior { get }
```

## Discussion

Items with this behavior may not be removed or moved by the user. They will be placed before other customizatable items. Use this behavior for the most important items that users need for the app to do common functionality.

## See Also

### Getting customization behaviors

static var `default`: ToolbarCustomizationBehavior

The default customization behavior.

static var reorderable: ToolbarCustomizationBehavior

The reorderable customization behavior.

