

- Audio Toolbox
- AUAudioUnitFactory
-  createAudioUnit(with:) 

Instance Method

# createAudioUnit(with:)

Creates an instance of an extension’s audio unit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func createAudioUnit(with desc: AudioComponentDescription) throws -> AUAudioUnit
```

**Required**

## Parameters 

`desc`  

The description of the audio component.

## Return Value

An instance of the extension’s audio unit.

## Discussion

This method is called only once per factory instance.

Note

In non-ARC code, “create” methods return unretained objects (unlike C “create” functions). In this scenario, you should return an object with a reference count of 1, but autoreleased.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

