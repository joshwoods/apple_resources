

- UIKit
- UIConfigurationState
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses custom states by key.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
subscript(key: UIConfigurationStateCustomKey) -> AnyHashable? { get set }
```

**Required**

## See Also

### Managing configuration states

var traitCollection: UITraitCollection

The traits that describe the current layout environment of the view, such as the user interface style and layout direction.

**Required**

