

- SpriteKit
- SKReferenceNode
-  init(url:) 

Initializer

# init(url:)

Creates a reference node from a URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**watchOS**

``` source
convenience init(url referenceURL: URL)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(url referenceURL: URL)
```

## Parameters 

`referenceURL`  

The URL of the reference node.

## Return Value

A newly initialized reference node.

## Discussion

This intializer is for loading archives that reside outside of the app bundle.

## See Also

### Initializers

init(url: URL?)

Initializes a reference node from a URL.

convenience init(fileNamed: String)

Creates a reference node from a file in the app’s main bundle.

init(fileNamed: String?)

Initializes a reference node from a file in the app’s main bundle.

init?(coder: NSCoder)

A method that initializes a reference node from an archive.

