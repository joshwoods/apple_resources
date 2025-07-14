

- BrowserEngineKit
- BETextInput
-  insert(\_:) 

Instance Method

# insert(\_:)

Inserts the given `text` or one of it’s alternative texts available on `alternatives`

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func insert(_ alternatives: BETextAlternatives)
```

**Required**

## Mentioned in 

Integrating custom browser text views with UIKit

## See Also

### Text alternatives

func alternativesForSelectedText() -> [BETextAlternatives]?

Returns the text alternatives that are available to the text input object.

**Required**

func add(BETextAlternatives)

Adds text alternatives to the text input object for the current selection

**Required**

