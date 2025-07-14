

- BrowserEngineKit
- BETextInput
-  add(\_:) 

Instance Method

# add(\_:)

Adds text alternatives to the text input object for the current selection

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func add(_ alternatives: BETextAlternatives)
```

**Required**

## Mentioned in 

Integrating custom browser text views with UIKit

## See Also

### Text alternatives

func alternativesForSelectedText() -> [BETextAlternatives]?

Returns the text alternatives that are available to the text input object.

**Required**

func insert(BETextAlternatives)

Inserts the given `text` or one of it’s alternative texts available on `alternatives`

**Required**

