

- ManagedSettings
- ManagedSettingsStore
-  init(named:) 

Initializer

# init(named:)

Creates a new instance of a store with a custom name.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
convenience init(named name: ManagedSettingsStore.Name)
```

## Parameters 

`name`  

A unique name for the store.

## Discussion

Each store contains the settings that the client app applies. If the client app doesn’t explicitly apply a setting, the default value is `nil`. Using `.default` is akin to calling `ManagedSettingsStore()`.

