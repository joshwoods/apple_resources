

- SwiftUI
-  ForEach 

Structure

# ForEach

A structure that computes views on demand from an underlying collection of identified data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct ForEach where Data : RandomAccessCollection, ID : Hashable
```

## Mentioned in 

Creating performant scrollable stacks

Grouping data with lazy stack views

Displaying data in lists

Picking container views for your content

## Overview

Use `ForEach` to provide views based on a RandomAccessCollection of some data type. Either the collection’s elements must conform to Identifiable or you need to provide an `id` parameter to the `ForEach` initializer.

The following example creates a `NamedFont` type that conforms to Identifiable, and an array of this type called `namedFonts`. A `ForEach` instance iterates over the array, producing new Text instances that display examples of each SwiftUI Font style provided in the array.

```
private struct NamedFont: Identifiable {
    let name: String
    let font: Font
    var id: String { name }
}

private let namedFonts: [NamedFont] = [
    NamedFont(name: "Large Title", font: .largeTitle),
    NamedFont(name: "Title", font: .title),
    NamedFont(name: "Headline", font: .headline),
    NamedFont(name: "Body", font: .body),
    NamedFont(name: "Caption", font: .caption)
]

var body: some View {
    ForEach(namedFonts) { namedFont in
        Text(namedFont.name)
            .font(namedFont.font)
    }
}
```

Some containers like List or LazyVStack will query the elements within a for each lazily. To obtain maximal performance, ensure that the view created from each element in the collection represents a constant number of views.

For example, the following view uses an if statement which means each element of the collection can represent either 1 or 0 views, a non-constant number.

```
ForEach(namedFonts) { namedFont in
    if namedFont.name.count != 2 {
        Text(namedFont.name)
    }
}
```

You can make the above view represent a constant number of views by wrapping the condition in a VStack, an HStack, or a ZStack.

```
ForEach(namedFonts) { namedFont in
    VStack {
        if namedFont.name.count != 2 {
            Text(namedFont.name)
        }
    }
}
```

When enabling the following launch argument, SwiftUI will log when it encounters a view that produces a non-constant number of views in these containers:

```
-LogForEachSlowPath YES
```

## Topics

### Creating a collection

init(Data)

Creates an instance that uniquely identifies and creates table rows across updates based on the identity of the underlying data.

init(_:content:)

Creates an instance that uniquely identifies and creates map content across updates based on the identity of the underlying data.

init(_:id:content:)

Creates an instance that uniquely identifies and creates map content across updates based on the provided key path to the underlying data’s identifier.

### Creating an editable collection

init&lt;C, R>(Binding&lt;C>, editActions: EditActions&lt;C>, content: (Binding&lt;C.Element>) -> R)

Creates an instance that uniquely identifies and creates views across updates based on the identity of the underlying data.

init&lt;C, R>(Binding&lt;C>, id: KeyPath&lt;C.Element, ID>, editActions: EditActions&lt;C>, content: (Binding&lt;C.Element>) -> R)

Creates an instance that uniquely identifies and creates views across updates based on the identity of the underlying data.

### Accessing content

var content: (Data.Element) -> Content

A function to create content on demand using the underlying data.

var data: Data

The collection of underlying identified data that SwiftUI uses to create views dynamically.

### Initializers

init&lt;V>(sections: V, content: (SectionConfiguration) -> Content)

Creates an instance that uniquely identifies and creates views across updates based on the sections of a given view.

init&lt;V>(subviews: V, content: (Subview) -> Content)

Creates an instance that uniquely identifies and creates views across updates based on the subviews of a given view.

### Default Implementations

AttachmentContent Implementations

## Relationships

### Conforms To

- AccessibilityRotorContent

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `AccessibilityRotorContent`.

- AttachmentContent
- ChartContent
- Copyable
- DynamicMapContent
- DynamicTableRowContent

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `TableRowContent`.

- DynamicViewContent

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `View`.

- MapContent
- TabContent

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `TabContent`.

- TableRowContent

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `TableRowContent`.

- View

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `View`.

## See Also

### Iterating over dynamic data

struct ForEachSectionCollection

A collection which allows a view to be treated as a collection of its sections in a for each loop.

struct ForEachSubviewCollection

A collection which allows a view to be treated as a collection of its subviews in a for each loop.

protocol DynamicViewContent

A type of view that generates views from an underlying collection of data.

