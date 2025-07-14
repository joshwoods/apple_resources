

- RealityKit
- AnimationLibraryComponent
-  unkeyedResources 

Instance Property

# unkeyedResources

The library’s animation resources that don’t have a queryable name.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var unkeyedResources: [AnimationResource]? { get }
```

## Return Value

An array of the animation resources that don’t have a key; otherwise, `nil`.

## See Also

### Accessing animations

var animations: AnimationLibraryComponent.AnimationCollection

The collection of animations an entity can play.

var defaultAnimation: AnimationResource?

The default animation resource.

var defaultKey: String?

The name of the default animation resource.

