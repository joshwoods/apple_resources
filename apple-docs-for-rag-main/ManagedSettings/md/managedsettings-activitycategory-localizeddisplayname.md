

- ManagedSettings
- ActivityCategory
-  localizedDisplayName 

Instance Property

# localizedDisplayName

A localized display name for the category.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
let localizedDisplayName: String?
```

## Discussion

In an extension that provides shield configurations, this property provides the category’s name. When you access this property outside that extension, the value is `nil`. See `ShieldConfigurationDataSource` in the `ManagedSettingsUI` framework for more information.

## See Also

### Accessing Category Identifiers

let token: ActivityCategoryToken?

An opaque representation of a category of activities.

