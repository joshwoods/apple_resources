

- UIKit
- UIPrinter
-  UIPrinter.CutterBehavior 

Enumeration

# UIPrinter.CutterBehavior

Constants that specify the cutter behavior of a roll-fed printer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum CutterBehavior
```

## Topics

### Constants

case noCut

Don’t cut the paper.

case printerDefault

Use the printer’s default behavior.

case cutAfterEachPage

Cut the paper after each page.

case cutAfterEachCopy

Cut the paper after each copy of the document.

case cutAfterEachJob

Cut the paper after each print job finishes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

