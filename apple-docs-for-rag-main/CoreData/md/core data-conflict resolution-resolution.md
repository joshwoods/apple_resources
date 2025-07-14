

- Core Data
-  Conflict resolution 

API Collection

# Conflict resolution

Detect and resolve conflicts that occur when data is changed on multiple threads.

## Topics

### Conflict Management

class NSConstraintConflict

An encapsulation of conflicts that occur during an attempt to save a managed object.

class NSMergeConflict

An encapsulation of conflicts that occur during an attempt to save changes in a managed object context.

class NSMergePolicy

A policy object that you use to resolve conflicts between the persistent store and in-memory versions of managed objects.

class NSQueryGenerationToken

A token that indicates which generation of the persistent store is being accessed.

## See Also

### Background tasks

Using Core Data in the background

Use Core Data in both a single-threaded and multithreaded app.

Loading and Displaying a Large Data Feed

Consume data in the background, and lower memory use by batching imports and preventing duplicate records.

Batch processing

Use batch processes to manage large data changes.

