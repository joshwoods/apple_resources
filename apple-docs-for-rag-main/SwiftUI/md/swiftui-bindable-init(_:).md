

- SwiftUI
- Bindable
-  init(\_:) 

Initializer

# init(\_:)

Creates a bindable object from an observable object.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(_ wrappedValue: Value)
```

Available when `Value` conforms to `Observable`.

## Discussion

This initializer is equivalent to init(wrappedValue:), but is more succinct when when creating bindable objects nested within other expressions. For example, you can use the initializer to create a bindable object inline with code that declares a view that takes a binding as a parameter:

```
struct TitleEditView: View {
    @Environment(Book.self) private var book

    var body: some View {
        TextField("Title", text: Bindable(book).title)
    }
}
```

## See Also

### Creating a bindable value

init(wrappedValue: Value)

Creates a bindable object from an observable object.

init(projectedValue: Bindable&lt;Value>)

Creates a bindable from the value of another bindable.

