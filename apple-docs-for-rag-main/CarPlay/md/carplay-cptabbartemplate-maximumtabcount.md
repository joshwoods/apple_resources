

- CarPlay
- CPTabBarTemplate
-  maximumTabCount 

Type Property

# maximumTabCount

The maximum number of tabs that the template can display.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class var maximumTabCount: Int { get }
```

## Discussion

This property’s value depends on the app’s entitlements. At runtime, use this value to determine the maximum number of tabs that your tab bar can display.

## See Also

### Managing the Templates

var templates: [CPTemplate]

The tab bar’s templates.

func updateTemplates([CPTemplate])

Adds, removes, reorders, or updates the tab bar’s templates.

