

- CallKit
-  CXCallController 

Class

# CXCallController

A programmatic interface for interacting with and observing calls.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXCallController
```

## Mentioned in 

Making and receiving VoIP calls

## Overview

A CXCallController object interacts with calls by performing actions, which are represented by instances of CXCallAction subclasses. You can request that one or more actions be performed in a single CXTransaction object using the request(_:completion:) method. A transaction may be rejected by the system for one of the reasons listed in the CXErrorCodeRequestTransactionError.Code enumeration.

Each CXCallController object manages a CXCallObserver object, which can be accessed using the callObserver property. You can provide an object conforming to the CXCallObserverDelegate protocol to the call observer in order to be notified of any changes to active calls.

## Topics

### Creating New Call Controllers

convenience init()

Initializes a new call controller with a private, serial queue, which is used for calling completion blocks.

init(queue: dispatch_queue_t)

Initializes a new call controller with a specified queue, which is used for calling completion blocks.

### Accessing the Call Observer

var callObserver: CXCallObserver

Returns an observer for active calls.

### Requesting Transactions

func request(CXTransaction, completion: ((any Error)?) -> Void)

Requests that the actions in the specified transaction be asynchronously performed by the telephony provider.

func requestTransaction(with: CXAction, completion: ((any Error)?) -> Void)

Requests that the transaction that contains the specified action be asynchronously performed by the telephony provider.

func requestTransaction(with: [CXAction], completion: ((any Error)?) -> Void)

Requests that the transaction that contains the specified actions be asynchronously performed by the telephony provider.

### Errors

struct CXErrorCodeRequestTransactionError

enum Code

Error codes for the CallKit error domain.

let CXErrorDomainRequestTransaction: String

Domain for errors when requesting a transaction from a call controller.

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

### Outgoing calls

Sending End-to-End Encrypted VoIP Calls

Initiate VoIP calls when your server can’t determine whether an outgoing notification is a request for a VoIP call due to metadata encryption.

class CXTransaction

An object that contains zero or more action objects for a call controller to perform.

class CXStartCallAction

An encapsulation of the act of initiating an outgoing call.

