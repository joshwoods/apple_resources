

- ManagedAppDistribution
- ManagedAppView
-  defaultAppStorage(\_:) 

Instance Method

# defaultAppStorage(\_:)

The default store used by `AppStorage` contained within the view.

ManagedAppDistributionSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func defaultAppStorage(_ store: UserDefaults) -> some View
```

## Parameters 

`store`  

The user defaults to use as the default store for `AppStorage`.

## Discussion

If unspecified, the default store for a view hierarchy is `UserDefaults.standard`, but can be set a to a custom one. For example, sharing defaults between an app and an extension can override the default store to one created with `UserDefaults.init(suiteName:_)`.

