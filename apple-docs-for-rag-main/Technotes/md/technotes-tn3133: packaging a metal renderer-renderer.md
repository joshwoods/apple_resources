

- Technotes
-  TN3133: Packaging a Metal renderer 

Article

# TN3133: Packaging a Metal renderer

Distribute a Metal renderer in a Swift package.

## Overview

Several individual pieces make up a Metal renderer: The CPU-side app code, the GPU-side shaders, and the structures that the app code and the shaders share. Bundling these pieces together in a single Swift package is an excellent way to modularize a renderer for use in multiple projects. Read this technote to discover a Swift package structure that shares C structs between Swift and Metal code, and to learn how to access the compiled Metal source as a `MTLLibrary`.

## Configure the package manifest

The package structure that enables you to package Swift, Metal, and shared C sources in a single Swift package requires two Target declarations, as shown in the following example package manifest:

```
// swift-tools-version:5.5

import PackageDescription

let package = Package(
    name: "MyRenderer",
    products: [
        .library(
            name: "MyRenderer",
            targets: ["MyRenderer"]),
    ],
    targets: [
        // MyRenderer contains .swift and .metal files.
        .target(
            name: "MyRenderer",
            dependencies: ["MySharedTypes"]),

        // MySharedTypes contains a .h file nested inside of a folder named "include", and an empty .m file, specifying that the target should be compiled as an Obj-C target.
        .target(name: "MySharedTypes")
    ]
)
```

The `MyRenderer` target contains the Swift source files, as well as the Metal source files.

The `MySharedTypes` target contains the shared C structs within a header file. Store this header in the directory specified as the publicHeadersPath for this target, so that the header is accessible from the `MyRenderer` target. It’s also important to have at least one Obj-C, C, or C++ implementation file in this target.

Note

A target cannot have source files from both Swift and C-family languages, but it’s OK to have Swift and Metal sources in the same target because SwiftPM treats Metal files as resource files.

Add the `MySharedTypes` target as a dependency of the `MyRenderer` target to access the shared C structs in the `MyRenderer` target.

Here is a visual representation of the file structure described in the example above:

```
.
└── MyRenderer
    ├── Package.swift
    ├── README.md
    └── Sources
        ├── MyRenderer
        │   ├── Renderer.swift
        │   └── Shaders.metal
        └── MySharedTypes
            ├── SharedTypes.m
            └── include
                └── SharedTypes.h
```

## Accessing the shared C structs in Swift

Swift Package Manager creates a module that contains the C structs found in the publicHeadersPath, and because the Swift target is dependent on the C target, the C structs are directly accessible from Swift.

Continuing with the same naming from the example above, consider the following header located at `MyRenderer/Sources/MySharedTypes/include/SharedTypes.h`:

```
#ifndef SharedTypes_h
#define SharedTypes_h

#import 

typedef struct {
    vector_float2 position;
    vector_float4 color;
} AAPLVertex;

#endif /* SharedTypes_h */
```

The shared types are accessible in Swift files after importing the `MySharedTypes` module, for example:

```
import MySharedTypes

let vertex = AAPLVertex(position: .init(250, -250), color: .init(1, 0, 0, 1))
```

## Accessing the shared C structs in Metal

Using the same package structure defined above, the shared types are accessible in Metal files after importing the appropriate header file:

```
// A relative path to SharedTypes.h.
#import "../MySharedTypes/include/SharedTypes.h"

// Use any C types found in the imported header in this Metal file.
```

## Retrieving the precompiled Metal library

Swift Package Manager compiles the Metal source to a `.metallib` and stores it in the resource bundle of the target. This resource bundle is accessible from Swift through the `Bundle.module` static property.

To create a `MTLLibrary` from this bundle in the Swift target:

```
do {
  // device is a `MTLDevice`.
  let library = try device.makeDefaultLibrary(bundle: Bundle.module)
} catch {
  // Handle the error.
}
```

For more information about the `Bundle.module` static property, see Bundling Resources with a Swift Package.

## Introducing a custom Metal compilation step

You might want to invoke the `metal` command-line tool yourself, and provide it with arguments that fit your specific needs. For example, you could compile your Metal source with debug symbols to enable shader debugging in a client app.

To introduce a custom Metal compilation step to the build process, create a Swift Package Build Tool Plugin that invokes the `metal` command-line tool with custom arguments, precompiles a `.metallib`, and stores it in the target’s resources directory by specifying it as an output file of the build command. Then, apply the plugin to the target that contains your `.metal` files.

For more information about creating and applying a Swift Package Build Tool Plugin, see Create Swift Package plugins.

## Revision History

- **2022-11-08** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

