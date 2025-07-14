

- SwiftUI
-  ContainerValueKey 

Protocol

# ContainerValueKey

A key for accessing container values.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol ContainerValueKey
```

## Overview

You can create custom container values by extending the ContainerValues structure with new properties. First declare a new container value key type and specify a value for the required defaultValue property:

```
private struct MyContainerValueKey: ContainerValueKey {
    static let defaultValue: String = "Default value"
}
```

The Swift compiler automatically infers the associated Value type as the type you specify for the default value. Then use the key to define a new container value property:

```
extension ContainerValues {
    var myCustomValue: String {
        get { self[MyContainerValueKey.self] }
        set { self[MyContainerValueKey.self] = newValue }
    }
}
```

Clients of your container value never use the key directly. Instead, they use the key path of your custom container value property. To set the container value for a view, add the containerValue(_:_:) view modifier to that view:

```
MyView()
    .containerValue(\.myCustomValue, "Another string")
```

As a convenience, you can also define a dedicated view modifier to apply this container value:

```
extension View {
    func myCustomValue(_ myCustomValue: String) -> some View {
        containerValue(\.myCustomValue, myCustomValue)
}
```

This improves clarity at the call site:

```
MyView()
    .myCustomValue("Another string")
```

To read the container value, use `Group(subviews:)` on a containing view, and then access the container value on members of that collection.

```
@ViewBuilder var content: some View {
    Text("A").myCustomValue("Hello")
    Text("B").myCustomValue("World")
}

Group(subviews: content) { subviews in
    ForEach(subviews) { subview in
        Text(subview.containerValues.myCustomValue)
    }
}
```

In practice, this will mostly be used by views that contain multiple other views to extract information from their subviews. You could turn the example above into such a container view as follows:

```
struct MyContainer: View {
    var content: Content

    init(@ViewBuilder content: () -> Content) {
        self.content = content()
    }

    var body: some View {
        Group(subviews: content) { subviews in
            ForEach(subviews) { subview in
                // Display each view side-by-side with its custom value.
                HStack {
                    subview
                    Text(subview.containerValues.myCustomValue)
                }
            }
        }
    }
}
```

## Topics

### Associated Types

associatedtype Value

The type of value produced by the container value.

**Required**

### Type Properties

static var defaultValue: Self.Value

The default value of the container value.

**Required**

## See Also

### Accessing a container’s subviews

struct Subview

An opaque value representing a subview of another view.

struct SubviewsCollection

An opaque collection representing the subviews of view.

struct SubviewsCollectionSlice

func containerValue&lt;V>(WritableKeyPath&lt;ContainerValues, V>, V) -> some View

Sets a particular container value of a view.

struct ContainerValues

A collection of container values associated with a given view.

