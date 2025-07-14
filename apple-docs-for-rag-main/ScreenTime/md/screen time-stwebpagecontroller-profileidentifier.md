

- Screen Time
- STWebpageController
-  profileIdentifier 

Instance Property

# profileIdentifier

An optional identifier for the current browsing profile.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+

``` source
@MainActor
var profileIdentifier: STWebHistory.ProfileIdentifier? { get set }
```

## Discussion

The default value is `nil`. This identifier represents a profile and allows you to keep your browsing separate for topics like work, personal, or school. Using `nil` will report web history without a profile identifier. Web browsers with a “default” profile may want to use `nil` in order to match any web history reported prior to this API.

