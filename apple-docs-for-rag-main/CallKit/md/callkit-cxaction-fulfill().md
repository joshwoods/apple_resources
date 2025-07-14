

- CallKit
- CXAction
-  fulfill() 

Instance Method

# fulfill()

Reports the successful execution of the action.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func fulfill()
```

## Mentioned in 

Making and receiving VoIP calls

## Discussion

Calling this method sets the isComplete property value to true. Calling this method more than once or calling it after calling the fail() method has no effect.

You should only call this method from the implementation of a `CXProviderDelegate` method.

## See Also

### Completing Actions

func fail()

Reports the failed execution of the action.

