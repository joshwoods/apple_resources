

- AppKit
- NSParagraphStyle
-  default 

Type Property

# default

The default paragraph style.

macOS 10.0+

``` source
@NSCopying
class var `default`: NSParagraphStyle { get }
```

## Discussion

The default paragraph style has the following default values:

| Subattribute    | Default                                       |
|-----------------|-----------------------------------------------|
| Alignment       | `NSNaturalTextAlignment`                      |
| Tab stops       | 12 left-aligned tabs, spaced by `28.0` points |
| Line break mode | `NSLineBreakByWordWrapping`                   |
| All others      | `0.0`                                         |

See individual method descriptions for explanations of each subattribute.

