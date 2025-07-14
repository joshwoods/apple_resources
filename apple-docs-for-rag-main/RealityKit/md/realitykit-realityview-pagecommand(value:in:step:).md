

- RealityKit
- RealityView
-  pageCommand(value:in:step:) 

Instance Method

# pageCommand(value:in:step:)

Steps a value through a range in response to page up or page down commands.

RealityKitSwiftUItvOS 14.3+

``` source
nonisolated
func pageCommand(
    value: Binding,
    in bounds: ClosedRange,
    step: V = 1
) -> some View where V : BinaryInteger
```

## Parameters 

`value`  

A `Binding` to the value to modify when the user pages up or down.

`bounds`  

A closed range that specifies the upper and lower bounds of `value`.

`step`  

The amount by which to increment or decrement `value`. Defaults to 1.

## Discussion

Use this command to step through sections of a data model associated with a view by providing a binding to a value, a range, and step. If taking another step would cause the value to exceed the bounds, then the value remains unchanged.

On tvOS, the user triggers ‘pageUp’ and ‘pageDown’ commands by pressing a dedicated button on a connected remote. For example, you can let a user page through a TV programming guide using the channel buttons:

```
struct GuideView: View {
    @State private var pageOffset: Int = 0

    var body: some View {
        GuideContent(at: pageOffset)
            .pageCommand(
                value: $pageOffset,
                in: 0...9,
                step: 1)
    }
}
```

