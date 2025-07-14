

- FinanceKitUI
- TransactionPicker
-  onPreferenceChange(\_:perform:) 

Instance Method

# onPreferenceChange(\_:perform:)

Adds an action to perform when the specified preference key’s value changes.

FinanceKitUISwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func onPreferenceChange(
    _ key: K.Type = K.self,
    perform action: @escaping (K.Value) -> Void
) -> some View where K : PreferenceKey, K.Value : Equatable
```

## Parameters 

`key`  

The key to monitor for value changes.

`action`  

The action to perform when the value for `key` changes. The `action` closure passes the new value as its parameter.

## Return Value

A view that triggers `action` when the value for `key` changes.

