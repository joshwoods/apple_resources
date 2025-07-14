

- Assignables
- AssignableDocumentView
-  accessibilityHint(\_:isEnabled:) 

Instance Method

# accessibilityHint(\_:isEnabled:)

Communicates to the user what happens after performing the view’s action.

AssignablesSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityHint(
    _ hint: Text,
    isEnabled: Bool
) -> ModifiedContent
```

## Parameters 

`hint`  

The accessibility hint to apply.

`isEnabled`  

If true the accessibility hint is applied; otherwise the accessibility hint is unchanged.

## Discussion

Provide a hint in the form of a brief phrase, like “Purchases the item” or “Downloads the attachment”.

Note

On macOS, if the view does not have an action and it has been made into a container with `accessibilityElement(children: .contain)`, this will be used to describe the container. For example, if the container is for a graph, the hint could be “graph”.

