

- SwiftUI
- ImageRenderer
-  objectWillChange 

Instance Property

# objectWillChange

A publisher that informs subscribers of changes to the image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final let objectWillChange: PassthroughSubject
```

## Discussion

The renderer’s ObjectWillChangePublisher publishes `Void` elements. Subscribers should interpret any event as indicating that the contents of the image may have changed.

