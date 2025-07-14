

- TipKit
- Tip
-  image 

Instance Property

# image

The image associated with the tip.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var image: Image? { get }
```

**Required**

## Discussion

Use this property to display an icon to the left of the `title` and `message` of your tip. This property is `Optional` and defaults to a value of `nil`.

## See Also

### Setting tip content

var title: Text

A title that names the tip.

**Required**

var message: Text?

A short description of how to use the tip’s feature.

**Required**

var id: String

The tip’s unique identifier.

**Required**

