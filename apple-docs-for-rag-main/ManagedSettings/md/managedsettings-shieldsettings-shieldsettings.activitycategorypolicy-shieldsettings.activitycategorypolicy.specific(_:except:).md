

- ManagedSettings
- ShieldSettings
- ShieldSettings.ActivityCategoryPolicy
-  ShieldSettings.ActivityCategoryPolicy.specific(\_:except:) 

Case

# ShieldSettings.ActivityCategoryPolicy.specific(\_:except:)

A policy that indicates the device shields specific categories of activity, with some exceptions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case specific(
    Set,
    except: Set> = []
)
```

## Discussion

List categories you want to shield in the first parameter. Use the `except` parameter to specify apps and websites not to shield, even if they’re in the categories that you list. Your app can shield up to 50 category tokens and specify up to 50 application or web domain tokens exceptions at once.

## See Also

### Shielding Categories

case none

A policy that indicates the device doesn’t shield any content.

case all(except: Set&lt;Token&lt;Activity>>)

A policy that indicates the device shields all apps and websites, except content that you specify.

