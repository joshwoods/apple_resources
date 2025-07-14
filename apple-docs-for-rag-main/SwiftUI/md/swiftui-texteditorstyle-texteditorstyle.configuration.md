

- SwiftUI
- TextEditorStyle
-  TextEditorStyle.Configuration 

Type Alias

# TextEditorStyle.Configuration

The properties of a text editor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
typealias Configuration = TextEditorStyleConfiguration
```

## See Also

### Creating custom styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a text editor.

**Required**

associatedtype Body : View

A view that represents the body of a text editor.

**Required**

