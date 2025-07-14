

- SwiftUI
- FormStyle
-  FormStyle.Configuration 

Type Alias

# FormStyle.Configuration

The properties of a form instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias Configuration = FormStyleConfiguration
```

## Discussion

You receive a `configuration` parameter of this type — which is an alias for the FormStyleConfiguration type — when you implement the required makeBody(configuration:) method in a custom form style implementation.

## See Also

### Creating custom form styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a form.

**Required**

associatedtype Body : View

A view that represents the appearance and interaction of a form.

**Required**

