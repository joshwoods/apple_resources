

- RealityKit
- ModelSortGroup
-  ModelSortGroup.PlanarUIPlacement 

Enumeration

# ModelSortGroup.PlanarUIPlacement

A set of predefined groups that indicate how the renderer draws a model relative to a planar mesh or a SwiftUI view that’s coplanar and overlapping.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum PlanarUIPlacement
```

### Overview

Use one of the predefined groups planarUIInline, planarUIAlwaysInFront, and planarUIAlwaysBehind to order virtual content relative to coincidental (coplanar and overlapping) app UI to avoid rendering artifacts.

### Placing virtual content relative to app UI

The scenario below shows a museum scene that has a green planar mesh entity, stacked between two SwiftUI View instances in a ZStack.

| **Actual View** | **Layout Illustration** |
|----|----|
|  |  |

```
ZStack {
   // A red UI layer.
   Color(.red).opacity(0.5)
       .frame(width: 700, height: 520, alignment: .center)
       .clipShape(RoundedRectangle(cornerRadius: 40))

   // A green plane with 0.9 opacity.
   RealityView { content in
       let greenPlane = Entity()
       let planeModel = ModelComponent(
           mesh: .generatePlane(width: 0.3, height: 0.2, cornerRadius: 0.01),
           materials: [UnlitMaterial(color: .green)]
       )
       greenPlane.components.set(planeModel)
       greenPlane.components.set(OpacityComponent(opacity: 0.9))

       // Set the model sort group to planarUIInline.
       let group = ModelSortGroup.planarUIInline
       greenPlane.components.set(ModelSortGroupComponent(group: group, order: 0))
       content.add(greenPlane)
   }
   .frame(depth: 0.0)

   // A UI with text and SF symbol.
   VStack {
       Text("Hello World").font(.system(size: 50))
       Image(systemName: "visionpro")
           .resizable()
           .foregroundColor(.yellow)
           .aspectRatio(contentMode: .fit)
           .frame(width: 80.0, height: 80.0)
   }
   .frame(width: 460, height: 240, alignment: .center)
   .offset(z: .ulpOfOne)
}
```

Use the planarUIInline group to draw the `greenPlane` entity according to its placement within the `ZStack`. The `greenPlane` draws over the red layer, and the text/symbol draws over the `greenPlane`.

```
let group = ModelSortGroup.planarUIAlwaysInline
greenPlane.components.set(ModelSortGroupComponent(group: group, order: 0))
```

Use the planarUIAlwaysInFront group to order the `greenPlane` after both UI layers. The `greenPlane` draws over both the text/symbol layer and the red layer.

```
let group = ModelSortGroup.planarUIAlwaysInFront
greenPlane.components.set(ModelSortGroupComponent(group: group, order: 0))
```

Use the planarUIAlwaysBehind group to order the `greenPlane` before both UI layers. The red layer and the text/symbol layer both draw over the `greenPlane`.

```
let group = ModelSortGroup.planarUIAlwaysBehind
greenPlane.components.set(ModelSortGroupComponent(group: group, order: 0))
```

## Topics

### Operators

static func == (ModelSortGroup.PlanarUIPlacement, ModelSortGroup.PlanarUIPlacement) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case alwaysBehind

Instructs the renderer to draw a model’s mesh behind a SwiftUI layer that’s coincident with the mesh.

case alwaysInFront

Instructs the renderer to draw a model’s mesh in front of a SwiftUI layer that’s coincident with the mesh.

case inlineUI

Instructs the renderer to draw a model’s mesh along with a SwiftUI layer that’s coincident with the mesh.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

