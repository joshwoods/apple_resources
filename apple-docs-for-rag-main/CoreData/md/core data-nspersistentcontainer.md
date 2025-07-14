

- Core Data
-  NSPersistentContainer 

Class

# NSPersistentContainer

A container that encapsulates the Core Data stack in your app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class NSPersistentContainer
```

## Mentioned in 

Setting up a Core Data stack manually

Setting Up Core Data with CloudKit

Setting up a Core Data stack

Using Core Data in the background

## Overview

NSPersistentContainer simplifies the creation and management of the Core Data stack by handling the creation of the managed object model (NSManagedObjectModel), persistent store coordinator (NSPersistentStoreCoordinator), and the managed object context (NSManagedObjectContext).

## Topics

### Creating a Container

convenience init(name: String)

Creates a container with the specified name.

init(name: String, managedObjectModel: NSManagedObjectModel)

Create a container with the specified name and managed object model.

### Getting the Container’s Configuration

var managedObjectModel: NSManagedObjectModel

The container’s managed object model.

var name: String

The container’s name.

var persistentStoreCoordinator: NSPersistentStoreCoordinator

The container’s persistent store coordinator.

### Accessing the Default Directory

class var defaultDirectoryURL: URL

The location of the directory that contains the persistent stores.

class func defaultDirectoryURL() -> URL

Returns the location of the directory that contains the persistent stores.

### Managing Persistent Stores

var persistentStoreDescriptions: [NSPersistentStoreDescription]

The descriptions of the container’s persistent stores.

func loadPersistentStores(completionHandler: (NSPersistentStoreDescription, (any Error)?) -> Void)

Loads the persistent stores.

### Acquiring Contexts

func newBackgroundContext() -> NSManagedObjectContext

Returns a new managed object context that executes on a private queue.

var viewContext: NSManagedObjectContext

The main queue’s managed object context.

### Performing Background Tasks

func performBackgroundTask((NSManagedObjectContext) -> Void)

Executes a closure on a private queue using an ephemeral managed object context.

func performBackgroundTask&lt;T>((NSManagedObjectContext) throws -> T) async rethrows -> T

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSPersistentCloudKitContainer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

