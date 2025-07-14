

- PackageDescription
- Resource
-  process(\_:localization:) 

Type Method

# process(\_:localization:)

Applies a platform-specific rules to the resource at the given path.

SwiftPM 5.3+

``` source
static func process(
    _ path: String,
    localization: Resource.Localization? = nil
) -> Resource
```

## Parameters 

`path`  

The path for a resource.

`localization`  

The explicit localization type for the resource.

## Return Value

A `Resource` instance.

## Discussion

Use the `process` rule to process resources at the given path according to the platform Swift Package Manager builds the target for. For example, Swift Package Manager may optimize image files for platforms that support such optimizations. If no optimization is available for a file type, Swift Package Manager copies the file.

If the given path represents a directory, Swift Package Manager applies the process rule recursively to each file in the directory.

If possible, use this rule instead of copy(_:).

## See Also

### Applying Rules

enum Localization

Defines the explicit type of localization for resources.

static func copy(String) -> Resource

Applies the copy rule to a resource at the given path.

