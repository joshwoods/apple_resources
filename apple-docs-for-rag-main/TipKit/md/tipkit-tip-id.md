

- TipKit
- Tip
-  id 

Instance Property

# id

The tip’s unique identifier.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var id: String { get }
```

**Required**

## Discussion

If you don’t provide a value, the system assigns the name of the type that conforms to the `Tip` protocol during initialization.

## See Also

### Setting tip content

var title: Text

A title that names the tip.

**Required**

var message: Text?

A short description of how to use the tip’s feature.

**Required**

var image: Image?

The image associated with the tip.

**Required**

