

- ManagedSettings
- ShieldSettings
-  webDomainCategories 

Type Property

# webDomainCategories

The metadata for the configuration that specifies categories of websites for the system to shield.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let webDomainCategories: SettingMetadata>
```

## Discussion

Use `webDomainCategories` to access the metadata for webDomainCategories. The default value is ShieldSettings.ActivityCategoryPolicy.none.

## See Also

### Blocking Categories of Apps and Websites

enum ActivityCategoryPolicy

Policies available for shielding activities based on their category.

var applicationCategories: ShieldSettings.ActivityCategoryPolicy&lt;Application>?

Categories of apps for the system to cover with a shielding view.

static let applicationCategories: SettingMetadata&lt;ShieldSettings.ActivityCategoryPolicy&lt;Application>>

The metadata for the configuration that specifies categories of apps for the system to cover with a shielding view.

var webDomainCategories: ShieldSettings.ActivityCategoryPolicy&lt;WebDomain>?

Categories of websites for the system to cover with a shielding view.

