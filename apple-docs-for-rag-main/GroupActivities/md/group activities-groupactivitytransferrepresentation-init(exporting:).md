

- Group Activities
- GroupActivityTransferRepresentation
-  init(exporting:) 

Initializer

# init(exporting:)

Creates a type that exports a group activity for the specified item.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
init(exporting: @escaping (Item) async throws -> ActivityType) where ActivityType : GroupActivity
```

## Parameters 

`exporting`  

A closure that creates the GroupActivity for the given item.

