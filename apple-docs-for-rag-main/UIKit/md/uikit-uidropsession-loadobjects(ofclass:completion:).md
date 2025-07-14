

- UIKit
- UIDropSession
-  loadObjects(ofClass:completion:) 

Instance Method

# loadObjects(ofClass:completion:)

Creates and loads a new instance of the specified class for each drag item in the session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func loadObjects(
    ofClass aClass: any NSItemProviderReading.Type,
    completion: @escaping ([any NSItemProviderReading]) -> Void
) -> Progress
```

**Required** Default implementation provided.

## Parameters 

`aClass`  

A class conforming to the NSItemProviderReading protocol.

`completion`  

The block that is executed after all objects are loaded.

## Return Value

An aggregate of the load progress for each object that is loaded.

## Mentioned in 

Making a view into a drop destination

## Discussion

You can use this method only in the drop interaction delegate’s implementation of the dropInteraction(_:performDrop:) method. This method is called after the user drops the items into the destination view.

The completion handler is called on the main queue. It provides an array of all objects created, in the same order that the drag items were added to the drag session.

## Default Implementations

### UIDropSession Implementations

func loadObjects&lt;T>(ofClass: T.Type, completion: ([T]) -> Void) -> Progress

