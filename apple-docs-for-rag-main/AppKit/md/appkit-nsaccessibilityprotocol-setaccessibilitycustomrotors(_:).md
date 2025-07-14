

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityCustomRotors(\_:) 

Instance Method

# setAccessibilityCustomRotors(\_:)

Sets the custom rotors of the current accessibility element.

macOS 10.13+

``` source
func setAccessibilityCustomRotors(_ accessibilityCustomRotors: [NSAccessibilityCustomRotor])
```

**Required**

## See Also

### Assigning Rotors

func accessibilityCustomRotors() -> [NSAccessibilityCustomRotor]

Returns the custom rotors of the current accessibility element.

**Required**

class NSAccessibilityCustomRotor

A context-sensitive function that helps VoiceOver users find the next instance of a related accessibility element.

