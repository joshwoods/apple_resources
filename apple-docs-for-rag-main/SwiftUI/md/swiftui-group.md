

- SwiftUI
-  Group 

Structure

# Group

A type that collects multiple instances of a content type — like views, scenes, or commands — into a single unit.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Group
```

## Overview

Use a group to collect multiple views into a single instance, without affecting the layout of those views, like an HStack, VStack, or Section would. After creating a group, any modifier you apply to the group affects all of that group’s members. For example, the following code applies the headline font to three views in a group.

```
Group {
    Text("SwiftUI")
    Text("Combine")
    Text("Swift System")
}
.font(.headline)
```

Because you create a group of views with a ViewBuilder, you can use the group’s initializer to produce different kinds of views from a conditional, and then optionally apply modifiers to them. The following example uses a `Group` to add a navigation bar title, regardless of the type of view the conditional produces:

```
Group {
    if isLoggedIn {
        WelcomeView()
    } else {
        LoginView()
    }
}
.navigationBarTitle("Start")
```

The modifier applies to all members of the group — and not to the group itself. For example, if you apply onAppear(perform:) to the above group, it applies to all of the views produced by the `if isLoggedIn` conditional, and it executes every time `isLoggedIn` changes.

Because a group of views itself is a view, you can compose a group within other view builders, including nesting within other groups. This allows you to add large numbers of views to different view builder containers. The following example uses a `Group` to collect 10 Text instances, meaning that the vertical stack’s view builder returns only two views — the group, plus an additional Text:

```
var body: some View {
    VStack {
        Group {
            Text("1")
            Text("2")
            Text("3")
            Text("4")
            Text("5")
            Text("6")
            Text("7")
            Text("8")
            Text("9")
            Text("10")
        }
        Text("11")
    }
}
```

You can initialize groups with several types other than View, such as Scene and ToolbarContent. The closure you provide to the group initializer uses the corresponding builder type (SceneBuilder, ToolbarContentBuilder, and so on), and the capabilities of these builders vary between types. For example, you can use groups to return large numbers of scenes or toolbar content instances, but not to return different scenes or toolbar content based on conditionals.

## Topics

### Creating a group

init(content:)

Creates an instance that generates Rotor content by combining, in order, all the Rotor content specified in the passed-in result builder.

### Initializers

init&lt;Base, Result>(sections: Base, transform: (SectionCollection) -> Result)

Constructs a group from the sections of the given view.

init&lt;Base, Result>(subviews: Base, transform: (SubviewsCollection) -> Result)

Constructs a group from the subviews of the given view.

## Relationships

### Conforms To

- AccessibilityRotorContent

  Conforms when `Content` conforms to `AccessibilityRotorContent`.

- Commands

  Conforms when `Content` conforms to `Commands`.

- Copyable
- CustomizableToolbarContent

  Conforms when `Content` conforms to `CustomizableToolbarContent`.

- MapContent
- Scene

  Conforms when `Content` conforms to `Scene`.

- TabContent

  Conforms when `Content` conforms to `TabContent`.

- TableColumnContent

  Conforms when `Content` conforms to `TableColumnContent`.

- TableRowContent

  Conforms when `Content` conforms to `TableRowContent`.

- ToolbarContent

  Conforms when `Content` conforms to `CustomizableToolbarContent`.

- View

  Conforms when `Content` conforms to `View`.

## See Also

### Grouping views into a container

Creating custom container views

Access individual subviews to compose flexible container views.

struct GroupElementsOfContent

Transforms the subviews of a given view into a resulting content view.

struct GroupSectionsOfContent

Transforms the sections of a given view into a resulting content view.

