

- ManagedAppDistribution
- ManagedAppView
-  focusedSceneValue(\_:\_:) 

Instance Method

# focusedSceneValue(\_:\_:)

Creates a new view that exposes the provided value to other views whose state depends on the active scene.

ManagedAppDistributionSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
nonisolated
func focusedSceneValue(
    _ keyPath: WritableKeyPath,
    _ value: T?
) -> some View
```

## Parameters 

`keyPath`  

The key path to associate `value` with when adding it to the existing table of published focus values.

`value`  

The focus value to publish, or `nil` if no value is currently available.

## Return Value

A modified representation of this view.

## Discussion

Use this method instead of `View/focusedValue(_:_:)` for values that must be visible regardless of where focus is located in the active scene. For example, if an app needs a command for moving focus to a particular text field in the sidebar, it could use this modifier to publish a button action that’s visible to command views as long as the scene is active, and regardless of where focus happens to be in it.

```
struct Sidebar: View {
    @FocusState var isFiltering: Bool

    var body: some View {
        VStack {
            TextField(...)
                .focused(when: $isFiltering)
                .focusedSceneValue(\.filterAction) {
                    isFiltering = true
                }
        }
    }
}

struct NavigationCommands: Commands {
    @FocusedValue(\.filterAction) var filterAction

    var body: some Commands {
        CommandMenu("Navigate") {
            Button("Filter in Sidebar") {
                filterAction?()
            }
        }
        .disabled(filterAction == nil)
    }
}

struct FilterActionKey: FocusedValuesKey {
    typealias Value = () -> Void
}

extension FocusedValues {
    var filterAction: (() -> Void)? {
        get { self[FilterActionKey.self] }
        set { self[FilterActionKey.self] = newValue }
    }
}
```

