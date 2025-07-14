

- Scripting Bridge
- SBElementArray
-  array(byApplying:) 

Instance Method

# array(byApplying:)

Returns an array containing the results of sending the specified message to each object in the receiver.

Mac Catalyst 13.0+macOS 10.5+

``` source
func array(byApplying selector: Selector) -> [Any]
```

## Parameters 

`selector`  

A selector identifying the message to be sent to each object in the array.

## Return Value

A new array containing the results of sending the `selector` message to each object in the receiver, starting with the first object and continuing through the element array to the last object.

## Discussion

The method identified by `selector` must not take any arguments and must return an Objective-C object. It should not have the side effect of modifying the receiving array. The order of the items in the result array corresponds to the order of the items in the original array.

## See Also

### Filtering an Element Array

func array(byApplying: Selector, with: Any) -> [Any]

Returns an array containing the results of sending the specified message to each object in the receiver.

