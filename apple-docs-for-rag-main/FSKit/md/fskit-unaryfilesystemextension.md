

- FSKit
-  UnaryFileSystemExtension 

Protocol

# UnaryFileSystemExtension

A protocol for implementing a minimal file system as an app extension.

macOS 15.4+

``` source
protocol UnaryFileSystemExtension : AppExtension
```

## Overview

Your app needs to do the following to implement a FSKit-compatible minimal file system:

1.  Create a subclass of FSUnaryFileSystem, which also conforms to FSUnaryFileSystemOperations.

2.  Implement a `@main` struct that conforms to the `UnaryFileSystemExtension` protocol. Your implementation of this protocol returns the type of class from step 1 as its FileSystem associated type, and returns an instance of it as the fileSystem property.

## Topics

### Associated Types

associatedtype FileSystem : FSUnaryFileSystem, FSUnaryFileSystemOperations

The type of file system your app extension provides.

**Required**

### Instance Properties

var fileSystem: Self.FileSystem

The instance of your file system type that your app extension provides.

**Required**

## Relationships

### Inherits From

- AppExtension

