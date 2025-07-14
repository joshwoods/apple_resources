

- Combine
- Publishers
- Publishers.Merge5
-  assign(to:on:) 

Instance Method

# assign(to:on:)

Assigns each element from a publisher to a property on an object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func assign(
    to keyPath: ReferenceWritableKeyPath,
    on object: Root
) -> AnyCancellable
```

Available when `Failure` is `Never`.

## Parameters 

`keyPath`  

A key path that indicates the property to assign. See Key-Path Expression in *The Swift Programming Language* to learn how to use key paths to specify a property of an object.

`object`  

The object that contains the property. The subscriber assigns the object’s property every time it receives a new value.

## Return Value

An AnyCancellable instance. Call cancel() on this instance when you no longer want the publisher to automatically assign the property. Deinitializing this instance will also cancel automatic assignment.

## Discussion

Use the assign(to:on:) subscriber when you want to set a given property each time a publisher produces a value.

In this example, the assign(to:on:) sets the value of the `anInt` property on an instance of `MyClass`:

```
class MyClass {
    var anInt: Int = 0 {
        didSet {
            print("anInt was set to: \(anInt)", terminator: "; ")
        }
    }
}

var myObject = MyClass()
let myRange = (0...2)
cancellable = myRange.publisher
    .assign(to: \.anInt, on: myObject)

// Prints: "anInt was set to: 0; anInt was set to: 1; anInt was set to: 2"
```

Important

The Subscribers.Assign instance created by this operator maintains a strong reference to `object`, and sets it to `nil` when the upstream publisher completes (either normally or with an error).

## See Also

### Connecting Simple Subscribers

func assign(to: inout Published&lt;Self.Output>.Publisher)

Republishes elements received from a publisher, by assigning them to a property marked as a publisher.

func sink(receiveCompletion: (Subscribers.Completion&lt;Self.Failure>) -> Void, receiveValue: (Self.Output) -> Void) -> AnyCancellable

Attaches a subscriber with closure-based behavior.

func sink(receiveValue: (Self.Output) -> Void) -> AnyCancellable

Attaches a subscriber with closure-based behavior to a publisher that never fails.

