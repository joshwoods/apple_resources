

- Swift
-  Calling Objective-C APIs Asynchronously 

Article

# Calling Objective-C APIs Asynchronously

Learn how functions and methods that take a completion handler are converted to Swift asynchronous functions.

## Overview

In Cocoa, methods that perform asynchronous operations take a completion handler as their last parameter, and the method calls that block after the operation finishes to return a result or an error. Swift 5.5 and later automatically translates Objective-C methods that take completion handlers into asynchronous methods using Swift’s native concurrency support, in addition to importing the callback-based version of the method into Swift. Because both Swift methods have the same behavior, they share the same page in the documentation.

For information about asynchronous functions, see Concurrency in The Swift Programming Language.

### Understand How Swift Imports Completion Handlers

Swift imports Objective-C methods that take a completion handler as two related Swift methods: a method that takes a closure, and an asynchronous method that doesn’t take a closure. For example, consider the present(completion:) method from PassKit. In Objective-C, it’s declared like this:

```
```

However, in Swift, it’s imported as two methods:

```
func present(completion: ((Bool) -> Void)? = nil)

func present() async -> Bool
```

The first version, `present(completion:)`, has a return type of `Void` and takes a completion handler. The second version, `present()`, returns a Boolean value and is an asynchronous method.

Methods whose completion handlers populate a NSError pointer parameter also become throwing methods in Swift, as described in About Imported Cocoa Error Parameters. The `NSError` parameter on an asynchronous throwing method must also be nullable, which indicates that the parameter is used only to communicate an error. For example, consider the write(_:timeout:completionHandler:) method from URLSessionStreamTask. In Objective-C, it’s declared like this:

```
```

As in the previous example, Swift imports this Objective-C method as two methods: an asynchronous method that takes a closure, and an asynchronous throwing method.

```
func write(
    _ data: Data, 
    timeout: TimeInterval, 
    completionHandler: @escaping (Error?) -> Void
)

func write(_ data: Data, timeout: TimeInterval) async throws
```

Methods whose completion handlers take multiple arguments become methods that return a tuple. For example, the sign(_:using:completion:) method from PassKit is declared like this in Objective-C:

```
```

In Swift it‘s imported as two methods, an asychronous method that takes a closure and an asynchronous throwing method that returns a tuple:

```
func sign(
    _ signData: Data, 
    using secureElementPass: PKSecureElementPass, 
    completion: @escaping (Data?, Data?, Error?) -> Void
)

func sign(_ signData: Data, 
    using secureElementPass: PKSecureElementPass
) async throws -> (Data, Data)
```

### Understand the Conversion Rules

The method that takes a completion handler must meet the following requirements:

- The method has a `void` return type.

- The block has a `void` return type.

- The block is called exactly once, on all possible paths of control flow.

If the method has only one parameter and its selector ends with one of the following suffixes, Swift imports the method as an asynchronous method:

- `WithCompletion`

- `WithCompletionHandler`

- `WithCompletionBlock`

- `WithReplyTo`

- `WithReply`

If the method has more than one parameter, and the last parameter’s selector piece is one of the following, Swift imports the method as an asynchronous method:

- `completion`

- `withCompletion`

- `completionHandler`

- `withCompletionHandler`

- `completionBlock`

- `withCompletionBlock`

- `replyTo`

- `withReplyTo`

- `reply`

- `replyTo`

The name of the Swift method is modified from the Objective-C method as follows:

- The selector piece for the completion handler is removed.

- If the selector starts with `get`, that prefix is removed and leading initialisms are converted to lowercase.

- If the selector ends with `Asynchronously`, that suffix is removed.

- If the method calls its completion handler with a nullable parameter, the asynchronous version in Swift is marked with the `@discardableResult` attribute.

## See Also

### Language Interoperability with Objective-C and C

Objective-C and C Code Customization

Apply macros to your Objective-C APIs to customize how they’re imported into Swift.

Migrating Your Objective-C Code to Swift

Learn the recommended steps to migrate your code.

Cocoa Design Patterns

Adopt and interoperate with Cocoa design patterns in your Swift apps.

Handling Dynamically Typed Methods and Objects in Swift

Cast instances of the Objective-C `id` type to a specific Swift type.

Using Objective-C Runtime Features in Swift

Use selectors and key paths to interact with dynamic Objective-C APIs.

Imported C and Objective-C APIs

Use native Swift syntax to interoperate with types and functions in C and Objective-C.

