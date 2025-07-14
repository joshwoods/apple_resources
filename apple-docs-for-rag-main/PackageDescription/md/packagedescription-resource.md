

- PackageDescription
-  Resource 

Structure

# Resource

A resource to bundle with the Swift package.

SwiftPM 5.3+

``` source
struct Resource
```

## Overview

If a Swift package declares a Swift tools version of 5.3 or later, it can include resource files. Similar to source code, Swift Package Manager scopes resources to a target, so you must put them into the folder that corresponds to the target they belong to. For example, any resources for the `MyLibrary` target must reside in `Sources/MyLibrary`. Use subdirectories to organize your resource files in a way that simplifies file identification and management. For example, put all resource files into a directory named `Resources`, so they reside at `Sources/MyLibrary/Resources`.

By default, Swift Package Manager handles common resources types for Apple platforms automatically. For example, you don’t need to declare XIB files, storyboards, Core Data file types, and asset catalogs as resources in your package manifest. However, you must explicitly declare other file types — for example, image files — as resources using the process(_:localization:) or copy(_:) rules. Alternatively, exclude resource files from a target by passing them to the target initializer’s exclude parameter.

To learn more about package resources, see doc:bundling-resources-with-a-swift-package.

## Topics

### Applying Rules

static func process(String, localization: Resource.Localization?) -> Resource

Applies a platform-specific rules to the resource at the given path.

enum Localization

Defines the explicit type of localization for resources.

static func copy(String) -> Resource

Applies the copy rule to a resource at the given path.

### Type Methods

static func embedInCode(String) -> Resource

Applies the embed rule to a resource at the given path.

## Relationships

### Conforms To

- Sendable

## See Also

### Configuring File Locations

var path: String?

The path of the target, relative to the package root.

var exclude: [String]

The paths to source and resource files that you don’t want to include in the target.

var sources: [String]?

The source files in this target.

var resources: [Resource]?

The explicit list of resource files in the target.

var publicHeadersPath: String?

The path to the directory that contains public headers of a C-family target.

