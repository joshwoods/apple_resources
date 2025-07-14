

- DeviceActivity
- DeviceActivityData
-  DeviceActivityData.WebDomainActivity 

Structure

# DeviceActivityData.WebDomainActivity

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct WebDomainActivity
```

## Topics

### Operators

static func == (DeviceActivityData.WebDomainActivity, DeviceActivityData.WebDomainActivity) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

var totalActivityDuration: TimeInterval

The total activity for this web domain.

var webDomain: WebDomain

The web domain that accumulated the activity.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

