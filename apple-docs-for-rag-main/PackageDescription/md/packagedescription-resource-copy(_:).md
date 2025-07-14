

- PackageDescription
- Resource
-  copy(\_:) 

Type Method

# copy(\_:)

Applies the copy rule to a resource at the given path.

SwiftPM 5.3+

``` source
static func copy(_ path: String) -> Resource
```

## Parameters 

`path`  

The path for a resource.

## Return Value

A `Resource` instance.

## Discussion

If possible, use process(_:localization:) and automatically apply optimizations to resources.

If your resources must remain untouched or must retain a specific folder structure, use the `copy` rule. It copies resources at the given `path`, as is, to the top level in the package’s resource bundle. If the given path represents a directory, Swift Package Manager preserves its structure.

## See Also

### Applying Rules

static func process(String, localization: Resource.Localization?) -> Resource

Applies a platform-specific rules to the resource at the given path.

enum Localization

Defines the explicit type of localization for resources.

