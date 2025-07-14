

- SecureElementCredential
- CredentialSession
-  Actor Implementations 

API Collection

# Actor Implementations

## Topics

### Instance Methods

func assertIsolated(@autoclosure () -> String, file: StaticString, line: UInt)

Stops program execution if the current task is not executing on this actor’s serial executor.

func assumeIsolated&lt;T>((isolated Self) throws -> T, file: StaticString, line: UInt) rethrows -> T

Assume that the current task is executing on this actor’s serial executor, or stop program execution otherwise.

func preconditionIsolated(@autoclosure () -> String, file: StaticString, line: UInt)

Stops program execution if the current task is not executing on this actor’s serial executor.

