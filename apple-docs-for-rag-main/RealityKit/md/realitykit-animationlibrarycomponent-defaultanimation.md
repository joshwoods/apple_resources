

- RealityKit
- AnimationLibraryComponent
-  defaultAnimation 

Instance Property

# defaultAnimation

The default animation resource.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var defaultAnimation: AnimationResource? { get }
```

## Discussion

The component looks up the resource by key if defaultKey is non-`nil` and the library contains an animation that the key identifies. Otherwise, the component returns the first entry in the library.

## See Also

### Accessing animations

var animations: AnimationLibraryComponent.AnimationCollection

The collection of animations an entity can play.

var unkeyedResources: [AnimationResource]?

The library’s animation resources that don’t have a queryable name.

var defaultKey: String?

The name of the default animation resource.

