

- CarPlay
- CPTabBarTemplate
-  templates 

Instance Property

# templates

The tab bar’s templates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var templates: [CPTemplate] { get }
```

## Discussion

The array contains the root template from each of the tab bar’s tabs. To add new templates to the tab bar, to remove or reorder existing templates, or to update a template’s tab bar appearance, use the updateTemplates(_:) method.

## See Also

### Managing the Templates

func updateTemplates([CPTemplate])

Adds, removes, reorders, or updates the tab bar’s templates.

class var maximumTabCount: Int

The maximum number of tabs that the template can display.

