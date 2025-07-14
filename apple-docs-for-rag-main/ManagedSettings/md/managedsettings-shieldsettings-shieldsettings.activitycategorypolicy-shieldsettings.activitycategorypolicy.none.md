

- ManagedSettings
- ShieldSettings
- ShieldSettings.ActivityCategoryPolicy
-  ShieldSettings.ActivityCategoryPolicy.none 

Case

# ShieldSettings.ActivityCategoryPolicy.none

A policy that indicates the device doesn’t shield any content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case none
```

## See Also

### Shielding Categories

case all(except: Set&lt;Token&lt;Activity>>)

A policy that indicates the device shields all apps and websites, except content that you specify.

case specific(Set&lt;ActivityCategoryToken>, except: Set&lt;Token&lt;Activity>>)

A policy that indicates the device shields specific categories of activity, with some exceptions.

