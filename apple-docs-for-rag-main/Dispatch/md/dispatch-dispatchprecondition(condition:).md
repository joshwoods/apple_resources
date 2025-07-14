

- Dispatch
-  dispatchPrecondition(condition:) 

Function

# dispatchPrecondition(condition:)

Checks a dispatch condition necessary for further execution.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
func dispatchPrecondition(condition: @autoclosure () -> DispatchPredicate)
```

## Parameters 

`condition`  

A dispatch predicate for the current context to check.

## Discussion

Use this function to detect conditions about the current execution context that must prevent the program from proceeding even in shipping code.

- In playgrounds and `-Onone` builds (the default for Xcode’s Debug configuration): if `condition` evaluates to `false`, stop program execution in a debuggable state.

- In `-O` builds (the default for Xcode’s Release configuration): if `condition` evaluates to `false`, stop program execution.

- In `-Ounchecked` builds, `condition` is not evaluated, but the optimizer may assume that it would evaluate to `true`. Failure to satisfy that assumption in `-Ounchecked` builds is a serious programming error.

## See Also

### Dispatch Objects

class DispatchObject

The base class for most dispatch types.

enum DispatchPredicate

Logical conditions to evaluate within a given execution context.

Dispatch Objects

The basic behaviors supported by all dispatch types.

