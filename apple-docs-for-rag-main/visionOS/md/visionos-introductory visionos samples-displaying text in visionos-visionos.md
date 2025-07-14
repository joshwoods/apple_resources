

- visionOS
- Introductory visionOS samples
-  Displaying text in visionOS 

Sample Code

# Displaying text in visionOS

Create styled text in a window using SwiftUI.

Download

visionOS 2.0+Xcode 16.0+

## Overview

This sample app uses SwiftUI views to display text in four distinct styles:

- Large title

- Subheadline

- Bold

- Regular with color

The following image shows how the scene renders in visionOS:

The app’s main view displays four lines of text by creating a Text instance for each line:

```
struct SwiftUIText: View {
    /// The amount of spacing between each text entry.
    let spacing: CGFloat = 30

    var body: some View {
        VStack(spacing: spacing) {
            // Set the style to large title.
            Text("This is a large title").font(.largeTitle)

            // Set the style to subheadline.
            Text("This is a subheadline text").font(.subheadline)

            // Format the text to bold.
            Text("This is a bold text").fontWeight(.bold)

            // Set the text's color to green.
            Text("This is a green text").foregroundStyle(.green)
        }
    }
}
```

SwiftUI provides the `Text` view and its modifiers, which the app uses to make each text appear unique.

## See Also

### Drawing text

Adding a depth effect to text in visionOS

Create text that expands out of a window using stacked SwiftUI text views.

