

- ARKit
- ReferenceObject
-  init(named:from:) 

Initializer

# init(named:from:)

Creates a reference object from a bundle.

visionOS 2.0+

``` source
init(
    named: String,
    from bundle: Bundle? = nil
) async throws
```

## Parameters 

`named`  

Name of object to load in bundle.

`bundle`  

Bundle to load from. If unspecified, defaults to the main bundle.

## See Also

### Creating reference objects

init(from: URL) async throws

Creates a reference object from a URL you provide.

