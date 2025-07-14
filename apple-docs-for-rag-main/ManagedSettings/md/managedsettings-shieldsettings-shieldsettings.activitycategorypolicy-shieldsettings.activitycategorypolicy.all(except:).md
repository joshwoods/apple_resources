

- ManagedSettings
- ShieldSettings
- ShieldSettings.ActivityCategoryPolicy
-  ShieldSettings.ActivityCategoryPolicy.all(except:) 

Case

# ShieldSettings.ActivityCategoryPolicy.all(except:)

A policy that indicates the device shields all apps and websites, except content that you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case all(except: Set> = [])
```

## Discussion

Your app can specify up to 50 application or web domain tokens exceptions at once.

## See Also

### Shielding Categories

case none

A policy that indicates the device doesn’t shield any content.

case specific(Set&lt;ActivityCategoryToken>, except: Set&lt;Token&lt;Activity>>)

A policy that indicates the device shields specific categories of activity, with some exceptions.

