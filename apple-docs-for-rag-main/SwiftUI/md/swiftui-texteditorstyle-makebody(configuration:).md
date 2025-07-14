

- SwiftUI
- TextEditorStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a text editor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the text editor.

## Discussion

The system calls this method for each TextEditor instance in a view hierarchy where this style is the current text editor style.

## See Also

### Creating custom styles

typealias Configuration

The properties of a text editor.

associatedtype Body : View

A view that represents the body of a text editor.

**Required**

