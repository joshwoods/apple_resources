

- ManagedSettings
- ShieldSettings
-  applicationCategories 

Type Property

# applicationCategories

The metadata for the configuration that specifies categories of apps for the system to cover with a shielding view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let applicationCategories: SettingMetadata>
```

## Discussion

The default value is ShieldSettings.ActivityCategoryPolicy.none.

## See Also

### Blocking Categories of Apps and Websites

enum ActivityCategoryPolicy

Policies available for shielding activities based on their category.

var applicationCategories: ShieldSettings.ActivityCategoryPolicy&lt;Application>?

Categories of apps for the system to cover with a shielding view.

var webDomainCategories: ShieldSettings.ActivityCategoryPolicy&lt;WebDomain>?

Categories of websites for the system to cover with a shielding view.

static let webDomainCategories: SettingMetadata&lt;ShieldSettings.ActivityCategoryPolicy&lt;WebDomain>>

The metadata for the configuration that specifies categories of websites for the system to shield.

