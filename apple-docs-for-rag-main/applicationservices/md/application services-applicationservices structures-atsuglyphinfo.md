

- Application Services
- ApplicationServices Structures
-  ATSUGlyphInfo 

Structure

# ATSUGlyphInfo

macOS 10.0+

``` source
struct ATSUGlyphInfo
```

## Topics

### Initializers

init()

init(glyphID: GlyphID, reserved: UInt16, layoutFlags: UInt32, charIndex: UniCharArrayOffset, style: ATSUStyle!, deltaY: Float32, idealX: Float32, screenX: Int16, caretX: Int16)

### Instance Properties

var caretX: Int16

var charIndex: UniCharArrayOffset

var deltaY: Float32

var glyphID: GlyphID

var idealX: Float32

var layoutFlags: UInt32

var reserved: UInt16

var screenX: Int16

var style: ATSUStyle!

