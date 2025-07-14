

- PackageDescription
- Resource
-  embedInCode(\_:) 

Type Method

# embedInCode(\_:)

Applies the embed rule to a resource at the given path.

SwiftPM 5.9+

``` source
static func embedInCode(_ path: String) -> Resource
```

## Parameters 

`path`  

The path for a resource.

## Return Value

A `Resource` instance.

## Discussion

You can use the embed rule to embed the contents of the resource into the executable code.

