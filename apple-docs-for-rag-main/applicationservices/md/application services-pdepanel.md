

- Application Services
-  PDEPanel 

Protocol

# PDEPanel

macOS 13.0+

``` source
protocol PDEPanel
```

## Topics

### Instance Methods

func panelKind() -> String

**Required**

func panelName() -> String

**Required**

func panelView() -> NSView?

**Required**

func ppdOptionKeyValueDidChange(String, ppdChoice: String)

**Required**

func printWindowWillClose(Bool)

func restoreValues()

**Required**

func saveValues()

**Required**

func shouldHide() -> Bool

**Required**

func shouldPrint() -> Bool

func shouldShowHelp() -> Bool

func summaryInfo() -> [String : String]?

**Required**

func supportedPPDOptionKeys() -> [String]?

func willShow()

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

