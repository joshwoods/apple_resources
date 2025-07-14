

- RealityKit
- AnimationLibraryComponent
-  defaultKey 

Instance Property

# defaultKey

The name of the default animation resource.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var defaultKey: String? { get set }
```

## Discussion

Returns `nil` if you don’t set a default animation, or if the component can’t find it.

## See Also

### Accessing animations

var animations: AnimationLibraryComponent.AnimationCollection

The collection of animations an entity can play.

var unkeyedResources: [AnimationResource]?

The library’s animation resources that don’t have a queryable name.

var defaultAnimation: AnimationResource?

The default animation resource.

