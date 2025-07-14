

- Metal
- MTLArchitecture
-  name 

Instance Property

# name

The name of a GPU device’s architecture.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var name: String { get }
```

## Discussion

The property’s value is equivalent to the output from the `metal-arch` command line tool on the same system.

```
% xcrun metal-arch
applegpu_g13s
```

Apps can use this property’s value to make decisions at runtime. For example, an app could retrieve a GPU-specific file from its developer’s content delivery network (CDN), such as a shader library or binary archive. See Shader Libraries and Shader Library and Archive Creation for more information.

