

- DeviceActivity
- DeviceActivityData
-  DeviceActivityData.CategoryActivity 

Structure

# DeviceActivityData.CategoryActivity

A categorized representation of a user’s application and web domain activity.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct CategoryActivity
```

## Topics

### Operators

static func == (DeviceActivityData.CategoryActivity, DeviceActivityData.CategoryActivity) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var applications: DeviceActivityResults&lt;DeviceActivityData.ApplicationActivity>

The user’s application activity that contributed to this category’s totalActivityDuration.

var category: ActivityCategory

The category of the activity.

var hashValue: Int

The hash value.

var totalActivityDuration: TimeInterval

The user’s total activity for this category.

var webDomains: DeviceActivityResults&lt;DeviceActivityData.WebDomainActivity>

The user’s web domain activity that contributed to this category’s totalActivityDuration.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

