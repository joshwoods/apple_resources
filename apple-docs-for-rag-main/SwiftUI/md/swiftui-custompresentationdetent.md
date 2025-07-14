

- SwiftUI
-  CustomPresentationDetent 

Protocol

# CustomPresentationDetent

The definition of a custom detent with a calculated height.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol CustomPresentationDetent
```

## Overview

You can create and use a custom detent with built-in detents.

```
extension PresentationDetent {
    static let bar = Self.custom(BarDetent.self)
    static let small = Self.height(100)
    static let extraLarge = Self.fraction(0.75)
}

private struct BarDetent: CustomPresentationDetent {
    static func height(in context: Context) -> CGFloat? {
        max(44, context.maxDetentValue * 0.1)
    }
}

struct ContentView: View {
    @State private var showSettings = false
    @State private var selectedDetent = PresentationDetent.bar

    var body: some View {
        Button("View Settings") {
            showSettings = true
        }
        .sheet(isPresented: $showSettings) {
            SettingsView(selectedDetent: $selectedDetent)
                .presentationDetents(
                    [.bar, .small, .medium, .large, .extraLarge],
                    selection: $selectedDetent)
        }
    }
}
```

## Topics

### Getting the height

static func height(in: Self.Context) -> CGFloat?

Calculates and returns a height based on the context.

**Required**

typealias Context

Information that you can use to calculate the height of a custom detent.

## See Also

### Configuring a sheet’s height

func presentationDetents(Set&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet.

func presentationDetents(Set&lt;PresentationDetent>, selection: Binding&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet, giving you programmatic control of the currently selected detent.

func presentationContentInteraction(PresentationContentInteraction) -> some View

Configures the behavior of swipe gestures on a presentation.

func presentationDragIndicator(Visibility) -> some View

Sets the visibility of the drag indicator on top of a sheet.

struct PresentationDetent

A type that represents a height where a sheet naturally rests.

struct PresentationContentInteraction

A behavior that you can use to influence how a presentation responds to swipe gestures.

