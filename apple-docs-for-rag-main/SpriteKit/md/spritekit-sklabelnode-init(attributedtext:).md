

- SpriteKit
- SKLabelNode
-  init(attributedText:) 

Initializer

# init(attributedText:)

Initializes a new label object with an attributed text string.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(attributedText: NSAttributedString?)
```

**watchOS**

``` source
convenience init(attributedText: NSAttributedString?)
```

## Parameters 

`attributedText`  

The attributed string from which to initialize the label.

## Return Value

A lable initialized from attributed text.

## Discussion

## See Also

### Creating a Label

init(fontNamed: String?)

Initializes a new label object with a specified font.

convenience init(text: String?)

Initializes a new label object with a text string.

