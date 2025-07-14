

- InputMethodKit
-  IMKServer 

Class

# IMKServer

The `IMKServer` class manages client connections to your input method. When you write the main function for your input method, you create an `IMKServer` object. You should never need to override this class.

macOS 10.5+

``` source
class IMKServer
```

## Topics

### Initializing a Server Object

init!(name: String!, bundleIdentifier: String!)

Creates and returns a server object from property list information contained in the provided bundle.

init!(name: String!, controllerClass: AnyClass!, delegateClass: AnyClass!)

Creates and returns a server object initialized with the provided parameters.

### Getting a Bundle for the Input Method

func bundle() -> Bundle!

Returns an `NSBundle` object for the input method.

### Constants

IMKModeDictionary

The input method mode dictionary key.

IMKControllerClass

The input method controller class key.

IMKDelegateClass

The input method delegate class key.

### Instance Methods

func lastKeyEventWasDeadKey() -> Bool

func paletteWillTerminate() -> Bool

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Classes

class IMKCandidates

The `IMKCandidates` class presents candidates to users and notifies the appropriate IMKInputController object when the user selects a candidate. **Candidates** are alternate characters for a given input sequence. The `IMKCandidates` class supports using a candidates window in your input method; using `IMKCandidates` is optional. Not all input methods require them.

class IMKInputController

The `IMKInputController` class provides a base class for custom input controller classes. The IMKServer class, which is allocated in the main function of an input method, creates an input controller object for each input session created by a client application. For every input session there is a corresponding `IMKInputController` object.

