

- TipKit
-  TipViewStyle 

Protocol

# TipViewStyle

A type that applies custom appearance to all tips within a view hierarchy.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol TipViewStyle
```

## Overview

To configure the current style for tips in a view hierarchy, use the tipViewStyle(_:) modifier and specify a type that conforms to `TipViewStyle`.

Customize the layout and style of your tips by creating a custom `TipViewStyle`:

```
struct HeadlineTipViewStyle: TipViewStyle {
    func makeBody(configuration: TipViewStyle.Configuration) -> some View {
        VStack(alignment: .leading) {
            HStack {
                Text("TIP").font(.system(.headline).smallCaps())
                Spacer()
                Button(action: { configuration.tip.invalidate(reason: .tipClosed) }) {
                    Image(systemName: "xmark").scaledToFit()
                }
            }

            Divider().frame(height: 1.0)

            HStack(alignment: .top) {
                configuration.image?
                    .resizable()
                    .aspectRatio(contentMode: .fit)
                    .frame(width: 48.0, height: 48.0)

                VStack(alignment: .leading, spacing: 8.0) {
                    configuration.title?.font(.headline)
                    configuration.message?.font(.subheadline)

                    ForEach(configuration.actions) { action in
                        Button(action: action.handler) {
                            action.label().foregroundStyle(.blue)
                        }
                    }
                }
            }
        }
    }
}
```

Use the tipViewStyle(_:) modifier to apply your style to all tips within a view hierarchy:

```
struct AddWorkoutView: View {
    var body: some View {
        VStack {
            TipView(AddWorkoutTip())
                .tipViewStyle(HeadlineTipViewStyle())

            Text("Workout Samples")
            WorkoutSampleList()
        }
    }
}
```

For UIKit and AppKit apps, the `viewStyle` property can be used for specifying a custom `TipViewStyle`:

```
let addWorkoutTipView = TipUIView(AddWorkoutTip())
addWorkoutTipView.viewStyle = HeadlineTipViewStyle()
addSubview(addWorkoutTipView)
```

## Topics

### Associated Types

associatedtype Body : View

The user interface element of the tip.

**Required**

### Instance Methods

func makeBody(configuration: Self.Configuration) -> Self.Body

A builder that makes the body of the tip view based on a style configuration.

**Required**

### Type Aliases

typealias Configuration

The tip style’s configuration.

### Type Properties

static var miniTip: MiniTipViewStyle

The default style for a tip view.

## Relationships

### Conforming Types

- MiniTipViewStyle

## See Also

### View Style

@MainActor @preconcurrency func tipViewStyle(_ style: some TipViewStyle) -> some View 

Sets the given style for TipView within the view hierarchy.

struct TipViewStyleConfiguration

The container type that holds a tip’s configuration.

struct MiniTipViewStyle

The default style for a TipView.

