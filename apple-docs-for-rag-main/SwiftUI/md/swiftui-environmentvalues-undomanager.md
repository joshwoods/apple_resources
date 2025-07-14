

- SwiftUI
- EnvironmentValues
-  undoManager 

Instance Property

# undoManager

The undo manager used to register a view’s undo operations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var undoManager: UndoManager? { get }
```

## Discussion

This value is `nil` when the environment represents a context that doesn’t support undo and redo operations. You can skip registration of an undo operation when this value is `nil`.

## See Also

### Storing document data in a class instance

protocol ReferenceFileDocument

A type that you use to serialize reference type documents to and from file.

struct ReferenceFileDocumentConfiguration

The properties of an open reference file document.

