

- SwiftUI
- PresentationSizing
-  sticky(horizontal:vertical:) 

Instance Method

# sticky(horizontal:vertical:)

Modifies self to be sticky in the specified dimensions — growing, but not shrinking.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func sticky(
    horizontal: Bool = false,
    vertical: Bool = false
) -> some PresentationSizing
```

## Parameters 

`horizontal`  

A boolean indicating whether to maintain the largest size horizontally

`vertical`  

A boolean indicating whether to maintain the largest size vertically

## Return Value

A modified version of self sticking to dimensions specified

## Discussion

If `sticky` is `.vertical`, the presentation can grow in the vertical and horizontal dimensions when its content size grows, but will not shrink in the vertical dimension when content size shrinks.

```
ContentView()
  .sheet(isPresented: $presentSheet) {
    MyDynamicSheetContent()
      .presentationSizing(
        .form.sticky(horizontal: false, vertical: true))
  }
```

See Also

fitted(horizontal:vertical:)

## See Also

### Creating custom presentation size

func fitted(horizontal: Bool, vertical: Bool) -> some PresentationSizing

func proposedSize(for: PresentationSizingRoot, context: PresentationSizingContext) -> ProposedViewSize

**Required**

