

- Application Services
- Core Printing
-  PMQualityMode 

Type Alias

# PMQualityMode

Constants that specify standard options for print quality.

macOS 10.0+

``` source
typealias PMQualityMode = UInt32
```

## Topics

### Constants

var kPMQualityLowest: Int

Specifies to use the lowest print quality available to the printer.

var kPMQualityInkSaver: Int

Specifies to use a mode that saves ink, even if it slows printing.

var kPMQualityDraft: Int

Specifies to print at the highest speed, with the amount of ink used as a secondary consideration.

var kPMQualityNormal: Int

Specifies a general usage mode that balances quality and speed.

var kPMQualityPhoto: Int

Specifies to optimize the quality of photos on the page, with speed not a concern.

var kPMQualityBest: Int

Specifies to get the best print quality for all objects and photos on a page.

var kPMQualityHighest: Int

Specifies to use the highest print quality available to the printer.

