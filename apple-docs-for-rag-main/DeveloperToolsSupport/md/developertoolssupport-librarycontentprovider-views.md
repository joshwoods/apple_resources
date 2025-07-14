

- DeveloperToolsSupport
- LibraryContentProvider
-  views 

Instance Property

# views

The SwiftUI views that you want to add to the Xcode library.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@LibraryContentBuilder
var views: [LibraryItem] { get }
```

**Required** Default implementation provided.

## Discussion

Xcode adds the LibraryItem instances returned by your implementation of this property to its Views library. The following restrictions apply:

- You must instantiate the library items inline.

- If specified, the item’s `title`, `category`, and `matchingSignature` must be static strings and not `nil`.

- The item’s `visible` value, if specified, must be a literal Boolean value.

- The item’s expression must be an instantiation. That is, it can’t be a reference.

## Default Implementations

### LibraryContentProvider Implementations

var views: [LibraryItem]

The SwiftUI views that you want to add to the Xcode library.

