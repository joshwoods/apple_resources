

- SwiftUI
-  GroupBox 

Structure

# GroupBox

A stylized view, with an optional label, that visually collects a logical grouping of content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
struct GroupBox where Label : View, Content : View
```

## Overview

Use a group box when you want to visually distinguish a portion of your user interface with an optional title for the boxed content.

The following example sets up a `GroupBox` with the label “End-User Agreement”, and a long `agreementText` string in a Text view wrapped by a ScrollView. The box also contains a Toggle for the user to interact with after reading the text.

```
var body: some View {
    GroupBox(label:
        Label("End-User Agreement", systemImage: "building.columns")
    ) {
        ScrollView(.vertical, showsIndicators: true) {
            Text(agreementText)
                .font(.footnote)
        }
        .frame(height: 100)
        Toggle(isOn: $userAgreed) {
            Text("I agree to the above terms")
        }
    }
}
```

## Topics

### Creating a group box

init(content: () -> Content)

Creates an unlabeled group box with the provided view content.

init(content: () -> Content, label: () -> Label)

Creates a group box with the provided label and view content.

init(_:content:)

Creates a group box with the provided view content and title.

### Creating a group box from a configuration

init(GroupBoxStyleConfiguration)

Creates a group box based on a style configuration.

### Deprecated initializers

init(label: Label, content: () -> Content)Deprecated

## Relationships

### Conforms To

- View

## See Also

### Grouping views into a box

func groupBoxStyle&lt;S>(S) -> some View

Sets the style for group boxes within this view.

