

- SwiftUI
-  LabeledContent 

Structure

# LabeledContent

A container for attaching a label to a value-bearing view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct LabeledContent
```

## Overview

The instance’s content represents a read-only or read-write value, and its label identifies or describes the purpose of that value. The resulting element has a layout that’s consistent with other framework controls and automatically adapts to its container, like a form or toolbar. Some styles of labeled content also apply styling or behaviors to the value content, like making Text views selectable.

The following example associates a label with a custom view and has a layout that matches the label of the Picker:

```
Form {
    LabeledContent("Custom Value") {
        MyCustomView(value: $value)
    }
    Picker("Selected Value", selection: $selection) {
        Text("Option 1").tag(1)
        Text("Option 2").tag(2)
    }
}
```

### Custom view labels

You can assemble labeled content with an explicit view for its label using the init(content:label:) initializer. For example, you can rewrite the previous labeled content example using a Text view:

```
LabeledContent {
    MyCustomView(value: $value)
} label: {
    Text("Custom Value")
}
```

The `label` view builder accepts any kind of view, like a Label:

```
LabeledContent {
    MyCustomView(value: $value)
} label: {
    Label("Custom Value", systemImage: "hammer")
}
```

For cases where adding a subtitle to the label is desired, use a view builder that creates multiple `Text` views where the first text represents the title and the second text represents the subtitle:

```
LabeledContent {
    MyCustomView(value: $value)
} label: {
    Text("Custom Value")
    Text("Custom Subtitle Value")
}
```

### Textual labeled content

You can construct labeled content with string values or formatted values to create read-only displays of textual values:

```
Form {
    Section("Information") {
        LabeledContent("Name", value: person.name)
        LabeledContent("Age", value: person.age, format: .number)
        LabeledContent("Height", value: person.height,
            format: .measurement(width: .abbreviated))
    }
    if !person.pets.isEmpty {
        Section("Pets") {
            ForEach(pet) { pet in
                LabeledContent(pet.species, value: pet.name)
            }
        }
    }
}
```

Wherever possible, SwiftUI makes this text selectable.

### Compositional elements

You can use labeled content as the label for other elements. For example, a NavigationLink can present a summary value for the destination it links to:

```
Form {
    NavigationLink(value: Settings.wifiDetail) {
        LabeledContent("Wi-Fi", value: ssidName)
    }
}
```

In some cases, the styling of views used as the value content is specialized as well. For example, while a Toggle in an inset group form on macOS is styled as a switch by default, it’s styled as a checkbox when used as a value element within a surrounding `LabeledContent` instance:

```
Form {
    LabeledContent("Source Control") {
        Toggle("Refresh local status automatically",
            isOn: $refreshLocalStatus)
        Toggle("Fetch and refresh server status automatically",
            isOn: $refreshServerStatus)
        Toggle("Add and remove files automatically",
            isOn: $addAndRemoveFiles)
        Toggle("Select files to commit automatically",
            isOn: $selectFiles)
    }
}
```

### Controlling label visibility

A label communicates the identity or purpose of the value, which is important for accessibility. However, you might want to hide the label in the display, and some controls or contexts may visually hide their label by default. The labelsHidden() modifier allows controlling that visibility. The following example hides both labels, producing only a group of the two value views:

```
Group {
    LabeledContent("Custom Value") {
        MyCustomView(value: $value)
    }
    Picker("Selected Value", selection: $selection) {
        Text("Option 1").tag(1)
        Text("Option 2").tag(2)
    }
}
.labelsHidden()
```

### Styling labeled content

You can set label styles using the labeledContentStyle(_:) modifier. You can also build custom styles using LabeledContentStyle.

## Topics

### Creating labeled content

init(_:content:)

Creates a labeled view that generates its label from a localized string key.

init(content: () -> Content, label: () -> Label)

Creates a standard labeled element, with a view that conveys the value of the element and a label.

init(_:value:)

Creates a labeled informational view.

init(_:value:format:)

Creates a labeled informational view from a formatted value.

init(LabeledContentStyleConfiguration)

Creates labeled content based on a labeled content style configuration.

## Relationships

### Conforms To

- Copyable
- View

  Conforms when `Label` conforms to `View` and `Content` conforms to `View`.

## See Also

### Grouping inputs

struct Form

A container for grouping controls used for data entry, such as in settings or inspectors.

func formStyle&lt;S>(S) -> some View

Sets the style for forms in a view hierarchy.

func labeledContentStyle&lt;S>(S) -> some View

Sets a style for labeled content.

