

- Open Directory
- ODSession
-  init(options:) 

Initializer

# init(options:)

Creates a session object directed over proxy to another host.

Mac CatalystmacOS 10.6+

``` source
init(options inOptions: [AnyHashable : Any]! = [:]) throws
```

## Parameters 

`inOptions`  

A dictionary of options to associate with the session. Can be `nil`.

## Return Value

The created session object.

## Discussion

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

class ODSession

An `ODSession` object serves as a Cocoa wrapper for an Open Directory session.

### Creating and Accessing Sessions

class func `default`() -> ODSession!

Returns a shared instance of the local session.

