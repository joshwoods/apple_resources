

- Core Text
-  CTFontPriority 

Type Alias

# CTFontPriority

The priority of font descriptors when resolving duplicates and sorting match results.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CTFontPriority = UInt32
```

## Discussion

Use the values of this enumeration for kCTFontPriorityAttribute.

## Topics

### Font Priority

var kCTFontPrioritySystem: Int

Priority of system fonts.

var kCTFontPriorityNetwork: Int

Priority of network fonts.

var kCTFontPriorityComputer: Int

Priority of computer local fonts.

var kCTFontPriorityUser: Int

Priority of local fonts.

var kCTFontPriorityDynamic: Int

Priority of fonts registered dynamically, not located in a standard location.

var kCTFontPriorityProcess: Int

Priority of fonts registered for the process.

## See Also

### Related Documentation

let kCTFontPriorityAttribute: CFString

The font priority used by font descriptors when resolving duplicates and sorting match results.

### Accessing Font Attributes

Font Attributes

The keys for accessing font attributes from a font descriptor.

enum CTFontOrientation

The intended rendering orientation of the font for obtaining glyph metrics.

enum CTFontFormat

The recognized format of the font.

