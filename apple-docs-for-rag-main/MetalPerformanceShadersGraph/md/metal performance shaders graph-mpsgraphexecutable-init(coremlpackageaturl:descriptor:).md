

- Metal Performance Shaders Graph
- MPSGraphExecutable
-  init(coreMLPackageAtURL:descriptor:) 

Initializer

# init(coreMLPackageAtURL:descriptor:)

Initialize the executable with the Core ML model package at the provided URL.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(
    coreMLPackageAtURL coreMLPackageURL: URL,
    descriptor compilationDescriptor: MPSGraphCompilationDescriptor?
)
```

## Parameters 

`coreMLPackageURL`  

The URL where to read the Core ML model package.

`compilationDescriptor`  

Compilation descriptor to be used to specialize, since the executable was created with a compilationDescriptor already this one overrides those settings to the extent it can.

