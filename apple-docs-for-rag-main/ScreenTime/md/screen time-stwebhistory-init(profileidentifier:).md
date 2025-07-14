

- Screen Time
- STWebHistory
-  init(profileIdentifier:) 

Initializer

# init(profileIdentifier:)

Creates a web history instance to delete web-usage data associated to the profile identifier you specify.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+

``` source
init(profileIdentifier: STWebHistory.ProfileIdentifier?)
```

## Parameters 

`profileIdentifier`  

The identifier of the current browsing profile.

## Discussion

The default value for `profileIdentifier` is `nil`. This identifier can be used to delete browsing history for a specific profile. Using `nil` will only delete web history reported without a profile identifier.

