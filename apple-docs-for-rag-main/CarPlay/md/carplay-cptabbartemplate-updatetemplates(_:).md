

- CarPlay
- CPTabBarTemplate
-  updateTemplates(\_:) 

Instance Method

# updateTemplates(\_:)

Adds, removes, reorders, or updates the tab bar’s templates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func updateTemplates(_ newTemplates: [CPTemplate])
```

## Parameters 

`newTemplates`  

An array of templates to display.

## Discussion

This method is multipurpose. Use it to add new templates to the tab bar, to remove and reorder existing templates, and to update a template’s tab bar appearance.

At runtime, use maximumTabCount to determine the maximum number of tabs the template can display. CarPlay throws an exception if the number of items in `newTemplates` exceeds this value.

Use a transactional approach when making changes to the tab bar. Retrieve the current set of templates using the templates property. Add, remove, reorder, or make appearance changes to one or more of array’s templates. For example, use the tabTitle property to update a template’s tab title, or set showsTabBadge to `true` to add an indicator to a template’s tab, then call this method with the updated array. CarPlay commits those changes and updates the tab bar.

CarPlay treats the array’s templates as root templates, each with its own navigation hierarchy. When a tab bar template is the rootTemplate of your app’s interface controller, and you use the controller to add and remove templates, CarPlay applies those changes to the selected tab’s navigation hierarchy.

CarPlay restricts the type of template you can use as a tab’s root template according to your app’s entitlements. Audio apps can use List and Grid templates only. All other categories of apps can use List, Grid, and Information templates as a tab’s root template. In addition, EV-charging, parking, and food ordering apps can use the Point of Interest template as a root template. These restrictions apply only to a tab’s root template. You can add other template types, like the Contact and Now Playing templates, on top of a tab’s root template using the methods that CPInterfaceController provides.

## See Also

### Managing the Templates

var templates: [CPTemplate]

The tab bar’s templates.

class var maximumTabCount: Int

The maximum number of tabs that the template can display.

