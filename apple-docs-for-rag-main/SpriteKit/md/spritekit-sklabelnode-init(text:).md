

- SpriteKit
- SKLabelNode
-  init(text:) 

Initializer

# init(text:)

Initializes a new label object with a text string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
convenience init(text: String?)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(text: String?)
```

## Parameters 

`text`  

The text to use to initialize the label node.

## Return Value

An initialized label object.

## Discussion

The label node’s font is set to Helvetica Neue Ultra Light, 32 point.

## See Also

### Creating a Label

init(fontNamed: String?)

Initializes a new label object with a specified font.

convenience init(attributedText: NSAttributedString?)

Initializes a new label object with an attributed text string.

