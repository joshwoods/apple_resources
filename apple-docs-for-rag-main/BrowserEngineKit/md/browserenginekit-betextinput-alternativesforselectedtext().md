

- BrowserEngineKit
- BETextInput
-  alternativesForSelectedText() 

Instance Method

# alternativesForSelectedText()

Returns the text alternatives that are available to the text input object.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func alternativesForSelectedText() -> [BETextAlternatives]?
```

**Required**

## Mentioned in 

Integrating custom browser text views with UIKit

## See Also

### Text alternatives

func add(BETextAlternatives)

Adds text alternatives to the text input object for the current selection

**Required**

func insert(BETextAlternatives)

Inserts the given `text` or one of it’s alternative texts available on `alternatives`

**Required**

