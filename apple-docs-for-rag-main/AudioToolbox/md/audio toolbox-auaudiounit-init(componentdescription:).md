

- Audio Toolbox
- AUAudioUnit
-  init(componentDescription:) 

Initializer

# init(componentDescription:)

Synchronously initializes a new audio unit object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(componentDescription: AudioComponentDescription) throws
```

## Parameters 

`componentDescription`  

The component to instantiate.

## Return Value

An initialized audio unit, or `nil` if initialization failed.

## Discussion

This is the convenience initializer.

A single audio unit subclass may implement multiple audio units—for example, an effect that can also function as a generator, or a cluster of related effects.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating an Audio Unit

init(componentDescription: AudioComponentDescription, options: AudioComponentInstantiationOptions) throws

Synchronously initializes a new audio unit object.

class func instantiate(with: AudioComponentDescription, options: AudioComponentInstantiationOptions, completionHandler: (AUAudioUnit?, (any Error)?) -> Void)

Asynchronously creates an audio unit instance.

