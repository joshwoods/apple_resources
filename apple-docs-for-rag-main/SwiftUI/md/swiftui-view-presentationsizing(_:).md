

- SwiftUI
- View
-  presentationSizing(\_:) 

Instance Method

# presentationSizing(\_:)

Sets the sizing of the containing presentation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func presentationSizing(_ sizing: some PresentationSizing) -> some View
```

## Parameters 

`sizing`  

A value dictating size to propose to presentation content and how the presentation responds to changes in content size.

## Discussion

Use this modifier to apply a PresentationSizing to a presentation like sheet(isPresented:onDismiss:content:). The `sizing` parameter defines the size proposed to the content, and the presentation adopts the returned size. The default value is `automatic`.

Sizings can be modified to fix their dimensions based on the content, and optionally be sticky.

See Also

fitted(horizontal:vertical:) and sticky(horizontal:vertical:).

Note

If the presentation’s root container is a `NavigationSplitView`, the proposed width only applies to the `detail` column. The `sidebar` and `content` column widths use system-provided values, or those from navigationSplitViewColumnWidth(_:) or navigationSplitViewColumnWidth(min:ideal:max:) modifiers.

For example, a presentation with facts about flowers could prefer `.page` sizing because its content is primarily informational. Since the user can choose different flowers from the picker, each with different lengths of information, the size is fitted vertically to size the sheet to the textual content, and vertically sticky is specified to prevent the presentation from changing size too frequently as the user changes selection.

```
struct ContentView: View {
    @State private var presentInfo = true

    var body: some View {
        ContentView.sheet(isPresented: $presentInfo) {
            VStack {
                Picker("Flower Species", selection: $flower) {
                    ForEach(Flower.allCases) {
                        Text($0.rawValue.uppercased()).tag($0)
                    }
                }
                Text(flower.emoji).font(.largeTitle)
                Text(flower.informationalText)
            }
            .frame(maxHeight: .infinity, alignment: .top)
            .padding()
            .presentationSizing(
                .page
                    .fitted(horizontal: false, vertical: true)
                    .sticky(horizontal: false, vertical: true))
        }
    }
}
```

## See Also

### Adapting a presentation size

func presentationCompactAdaptation(horizontal: PresentationAdaptation, vertical: PresentationAdaptation) -> some View

Specifies how to adapt a presentation to horizontally and vertically compact size classes.

func presentationCompactAdaptation(PresentationAdaptation) -> some View

Specifies how to adapt a presentation to compact size classes.

struct PresentationAdaptation

Strategies for adapting a presentation to a different size class.

protocol PresentationSizing

A type that defines the size of the presentation content and how the presentation size adjusts to its content’s size changing.

struct PresentationSizingRoot

A proxy to a view provided to the presentation with a defined presentation size.

struct PresentationSizingContext

Contextual information about a presentation.

