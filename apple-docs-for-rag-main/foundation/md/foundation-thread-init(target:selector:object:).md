

- Foundation
- Thread
-  init(target:selector:object:) 

Initializer

# init(target:selector:object:)

Returns an `NSThread` object initialized with the given arguments.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    target: Any,
    selector: Selector,
    object argument: Any?
)
```

## Parameters 

`target`  

The object to which the message specified by `selector` is sent.

`selector`  

The selector for the message to send to `target`. This selector must take only one argument and must not have a return value.

`argument`  

The single argument passed to the target. May be `nil`.

## Return Value

An `NSThread` object initialized with the given arguments.

## Discussion

The objects `target` and `argument` are retained during the execution of the detached thread. They are released when the thread finally exits.

## See Also

### Related Documentation

func start()

Starts the receiver.

### Initializing an NSThread Object

init()

Returns an initialized `NSThread` object.

