

- MapKit
-  LookAroundPreview 

Structure

# LookAroundPreview

A view that provides a Look Around preview for a specific geographic location.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+visionOS

``` source
@MainActor @preconcurrency
struct LookAroundPreview
```

## Overview

Use a `LookAroundPreview` to create preview imagery for a specific geographic location on the map that you can place in your view. In the following example, a travel recommendations app displays and styles a stack of Look Around previews it generates from an array of `ItineraryItem` structures that contain the location’s title and Look Around scene:

```
    struct LookAroundPreviewsView: View {
        let itinerary: [ItineraryItem]
        var body: some View {
            ScrollView {
                LazyVStack {
                    ForEach(itinerary) { item in
                        LookAroundPreview(initialScene: item.lookAroundScene)
                            .frame(height: 128)
                            .overlay(alignment: .bottomTrailing) {
                                Text(item.title)
                                    .font(.caption)
                                    .foregroundColor(.white)
                                    .padding()
                            }
                    }
                }
            }
        }
    }
```

To display a Look Around viewer a person can explore, apply a `lookAroundViewer` view modifier to a specific view, then add a control the user interacts with to display the Look Around viewer. In the following example, the `lookAroundViewer` view modifier observes a binding to Boolean value to determine whether to display the Look Around viewer.

```
    var lookAroundScene: MKLookAroundScene?

    @State private var isLookingAround: Bool = false

    var body: some View {
        MyInterestingView()
            .lookAroundViewer(isPresented: $isLookingAround, initialScene: lookAroundScene)
            .toolbar {
                ToolbarItem {
                    Button(action: { lookingAround = true }) {
                        Image(systemName: "binoculars")
                }
            }
        }   
    }
```

## Topics

### Creating a Look Around preview

init(initialScene: MKLookAroundScene?, allowsNavigation: Bool, showsRoadLabels: Bool, pointsOfInterest: PointOfInterestCategories, badgePosition: MKLookAroundBadgePosition)

Creates a Look Around preview with an initial scene, navigation, road label, points of interest, and badge position you specify.

init(scene: Binding&lt;MKLookAroundScene?>, allowsNavigation: Bool, showsRoadLabels: Bool, pointsOfInterest: PointOfInterestCategories, badgePosition: MKLookAroundBadgePosition)

Creates a Look Around preview with a binding to a scene, navigation, road label, points of interest, and badge position you specify.

## Relationships

### Conforms To

- Sendable
- View

