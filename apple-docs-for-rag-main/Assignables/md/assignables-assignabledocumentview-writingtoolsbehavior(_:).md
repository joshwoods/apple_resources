

- Assignables
- AssignableDocumentView
-  writingToolsBehavior(\_:) 

Instance Method

# writingToolsBehavior(\_:)

Specifies the Writing Tools behavior for text and text input in the environment.

AssignablesSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.4+

``` source
@MainActor @preconcurrency
func writingToolsBehavior(_ behavior: WritingToolsBehavior) -> some View
```

## Parameters 

`behavior`  

The Writing Tools behavior for text and text input in the environment.

## Return Value

A view preferring the specified Writing Tools behavior.

## Discussion

Use this view modifier to customize or disable the Writing Tools editing experience for `Text` (when selectable), `TextField`, and `TextEditor` views.

