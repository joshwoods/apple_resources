

- InputMethodKit
-  IMKCandidatesLocationHint 

Type Alias

# IMKCandidatesLocationHint

Hints that suggest where to place the candidates window.

macOS 10.5+

``` source
typealias IMKCandidatesLocationHint = Int
```

## Discussion

The Input Method Kit uses the hint to place the candidates window in a location that is in the vicinity of the hint location, but that also ensures that the candidates window is fully visible.

## Topics

### Constants

var kIMKLocateCandidatesAboveHint: Int

var kIMKLocateCandidatesBelowHint: Int

var kIMKLocateCandidatesLeftHint: Int

var kIMKLocateCandidatesRightHint: Int

## See Also

### Constants

typealias IMKCandidatePanelType

Types of candidates windows provide by the Input Method Kit.

IMKCandidatesOpacityAttributeName

The opacity level for a candidates window.

