

- ManagedSettings
-  BoundedSettingMetadata 

Structure

# BoundedSettingMetadata

Additional information about a bounded setting.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct BoundedSettingMetadata where Value : Comparable
```

## Topics

### Getting Metadata

let bounds: ClosedRange&lt;Value>

The range of values that a setting can accomodate.

let defaultValue: Value

The implicit value for a setting if your app doesn’t set a value.

## See Also

### Accessing Metadata

struct SettingMetadata

Additional information about a configurable setting.

