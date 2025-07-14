

- Core ML
- MLDictionaryFeatureProvider
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Subscript interface for the feature provider to pass through to the dictionary.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
subscript(featureName: String) -> MLFeatureValue? { get }
```

## See Also

### Accessing the Features

var dictionary: [String : MLFeatureValue]

The backing dictionary.

