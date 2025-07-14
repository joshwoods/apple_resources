

- SwiftUI
- Layout adjustments
-  Laying out a simple view 

Article

# Laying out a simple view

Create a view layout by adjusting the size of views.

## Overview

To create a layout for a view, start by composing a hierarchy of child views. Then, refine the size and spacing of the child views with configuration parameters, and by adding view modifiers, like those that affect a view’s frame and padding. To review how to compose layouts, see Building layouts with stack views.

### Establish a view hierarchy

The following example creates a view to display an incoming message from a messaging service. The view uses an HStack to collect a view that identifies the sender and another that provides the content of the message:

```
struct MessageRow: View {
    let message: Message

    var body: some View {
        HStack {
            ZStack {
                Circle()
                    .fill(Color.yellow)
                Text(message.initials)
            }

            Text(message.content)
        }
    }
}
```

The following screenshot of a `MessageRow` view includes a border that shows its bounds. Note the large size of the circle, which fills the space available to it:

When SwiftUI renders a view hierarchy, it recursively evaluates each child view: The parent view proposes a size to the child views it contains, and the child views respond with a computed size.

The `MessageRow` view proposes a size to its only child, the HStack, which is the full size proposed to it by its own parent. The stack proportionally divides this space between its child views, with system-default spacing between each child. This continues recursively:

- The ZStack proposes a size to its child views, the Circle and Text views.

- The Circle expands up to the size offered, while the Text takes just enough space for the string it contains.

- The ZStack returns the size of its largest child view, in this case the Circle.

When all child views have reported their size, the parent view renders them. For a hands-on approach to learning how the SwiftUI view hierarchy works, see the Building lists and navigation section in the Introducing SwiftUI tutorial.

### Limit the view size

In the example above, SwiftUI has built-in views that manage size in different ways, including views that:

- Expand to fill the space offered by their parent, like Color, LinearGradient, and Circle.

- Have an ideal size that varies according to their contents, like Text and the container views.

- Have an ideal size that never varies, like Toggle or DatePicker.

You can constrain a view to a fixed size by adding a frame modifier. For example, use the frame(width:height:alignment:) modifier to limit the width the circle to `40` points:

```
struct MessageRow: View {
    let message: Message

    var body: some View {
        HStack {
            ZStack {
                Circle()
                    .fill(Color.yellow)
                Text(message.initials)
            }
            .frame(width: 40)

            Text(message.content)
        }
    }
}
```

When you add a frame modifier, SwiftUI wraps the affected view, effectively adding a new view to the view hierarchy.

When SwiftUI evaluates this new hierarchy, the frame modifier fixes the width of the ZStack that it wraps by passing along the value you specified as its parameter. The remainder of the size evaluation proceeds as before, where the Circle now expands to fill a smaller space, constrained by the frame’s 40 point width. This enables the HStack to provide more space to its other child, which displays the message text.

### Position content with alignment

If you want the top of the circle aligned with the top of the message content text, you can refine the view by applying an alignment to the HStack. To position the content vertically within the stack, specify the `alignment` parameter to top:

```
struct MessageRow: View {
    let message: Message

    var body: some View {
        HStack(alignment: .top) {
            ZStack {
                Circle()
                    .fill(Color.yellow)
                Text(message.initials)
            }
            .frame(width: 40)

            Text(message.content)
        }
    }
}
```

With the alignment applied, you get an unexpected result. The tops of the views don’t appear to align:

However, if you select the circle in Xcode, or temporarily add a border to the circle, you can see the tops of the views do in fact align. For more information on inspecting the size of a view, see Inspecting view layout.

In the previous section, you applied a frame with only a width constraint. SwiftUI drew a circle limited by that width. But because the height was left unspecified, the circle’s frame separately expanded to fill the available height, even though that extra space had no visible impact on the rendered circle. You can resolve this problem by adding an explicit `height` parameter:

```
struct MessageRow: View {
    let message: Message

    var body: some View {
        HStack(alignment: .top) {
            ZStack {
                Circle()
                    .fill(Color.yellow)
                Text(message.initials)
            }
            .frame(width: 40, height: 40)

            Text(message.content)
        }
    }
}
```

The contents of the HStack are now top aligned, although the stack itself is centered in the `MessageRow` view as shown by the border displaying the row’s boundaries.

### Add padding to the view

To avoid visually crowding the outer edges of a view, add padding. This introduces a fixed amount of space along the specified edges, reducing the space available for the contents of the view by a corresponding amount. For example, you can use padding(_:_:) to add extra space along the horizontal edges of the HStack:

```
struct MessageRow: View {
    let message: Message

    var body: some View {
        HStack(alignment: .top) {
            ZStack {
                Circle()
                    .fill(Color.yellow)
                Text(message.initials)
            }
            .frame(width: 40, height: 40)

            Text(message.content)
        }
        .padding([.horizontal])
    }
}
```

The padding modifier defaults to system-standard spacing, although you can alternatively choose different values for the padding modifier. 

## See Also

### Finetuning a layout

Inspecting view layout

Determine the position and extent of a view using Xcode previews or by adding temporary borders.

