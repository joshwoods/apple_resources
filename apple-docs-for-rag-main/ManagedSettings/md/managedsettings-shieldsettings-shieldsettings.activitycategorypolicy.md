

- ManagedSettings
- ShieldSettings
-  ShieldSettings.ActivityCategoryPolicy 

Enumeration

# ShieldSettings.ActivityCategoryPolicy

Policies available for shielding activities based on their category.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
enum ActivityCategoryPolicy
```

## Topics

### Shielding Categories

case none

A policy that indicates the device doesn’t shield any content.

case all(except: Set&lt;Token&lt;Activity>>)

A policy that indicates the device shields all apps and websites, except content that you specify.

case specific(Set&lt;ActivityCategoryToken>, except: Set&lt;Token&lt;Activity>>)

A policy that indicates the device shields specific categories of activity, with some exceptions.

### Getting the Range

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (ShieldSettings.ActivityCategoryPolicy&lt;Activity>, ShieldSettings.ActivityCategoryPolicy&lt;Activity>) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Blocking Categories of Apps and Websites

var applicationCategories: ShieldSettings.ActivityCategoryPolicy&lt;Application>?

Categories of apps for the system to cover with a shielding view.

static let applicationCategories: SettingMetadata&lt;ShieldSettings.ActivityCategoryPolicy&lt;Application>>

The metadata for the configuration that specifies categories of apps for the system to cover with a shielding view.

var webDomainCategories: ShieldSettings.ActivityCategoryPolicy&lt;WebDomain>?

Categories of websites for the system to cover with a shielding view.

static let webDomainCategories: SettingMetadata&lt;ShieldSettings.ActivityCategoryPolicy&lt;WebDomain>>

The metadata for the configuration that specifies categories of websites for the system to shield.

