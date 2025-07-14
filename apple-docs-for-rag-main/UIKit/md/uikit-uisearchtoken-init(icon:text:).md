

- UIKit
- UISearchToken
-  init(icon:text:) 

Initializer

# init(icon:text:)

Creates a search token with the specified text and icon (if any).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(
    icon: UIImage?,
    text: String
)
```

## Parameters 

`icon`  

An image to display with the text.

`text`  

The text to display on the search token.

## Return Value

A new search token.

## See Also

### Creating a search token

var representedObject: Any?

The object represented by the search token.

