

- SwiftUI
- FormStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a form.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of the form.

## Return Value

A view that has behavior and appearance that enables it to function as a Form.

## See Also

### Creating custom form styles

typealias Configuration

The properties of a form instance.

associatedtype Body : View

A view that represents the appearance and interaction of a form.

**Required**

