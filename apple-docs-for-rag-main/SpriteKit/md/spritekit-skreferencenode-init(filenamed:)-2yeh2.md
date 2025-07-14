

- SpriteKit
- SKReferenceNode
-  init(fileNamed:) 

Initializer

# init(fileNamed:)

Initializes a reference node from a file in the app’s main bundle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**watchOS**

``` source
init(fileNamed fileName: String?)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init(fileNamed fileName: String?)
```

## Parameters 

`fileName`  

The name of a file stored in the app’s main bundle.

## Return Value

A newly initialized reference node.

## Discussion

This initializer is for loading files that reside inside of the app bundle.

## See Also

### Initializers

convenience init(url: URL)

Creates a reference node from a URL.

init(url: URL?)

Initializes a reference node from a URL.

convenience init(fileNamed: String)

Creates a reference node from a file in the app’s main bundle.

init?(coder: NSCoder)

A method that initializes a reference node from an archive.

