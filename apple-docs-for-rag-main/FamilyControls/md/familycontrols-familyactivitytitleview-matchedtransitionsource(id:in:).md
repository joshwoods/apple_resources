

- FamilyControls
- FamilyActivityTitleView
-  matchedTransitionSource(id:in:) 

Instance Method

# matchedTransitionSource(id:in:)

Identifies this view as the source of a navigation transition, such as a zoom transition.

FamilyControlsSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func matchedTransitionSource(
    id: some Hashable,
    in namespace: Namespace.ID
) -> some View
```

## Parameters 

`id`  

The identifier, often derived from the identifier of the data being displayed by the view.

`namespace`  

The namespace in which defines the `id`. New namespaces are created by adding an `Namespace` variable to a `View` type and reading its value in the view’s body method.

