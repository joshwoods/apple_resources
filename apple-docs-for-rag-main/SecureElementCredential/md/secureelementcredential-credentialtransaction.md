

- SecureElementCredential
-  CredentialTransaction 

Class

# CredentialTransaction

A transaction object for performing wired and contactless operations in SwiftUI views.

SecureElementCredentialSwiftUIiOS 18.1+iPadOS 18.1+

``` source
class CredentialTransaction
```

## Mentioned in 

Accessing and using secure element credentials

## Overview

Use the doc://com.apple.documentation/documentation/SwiftUI/View/transactionTask(\_:action) view modifier to create a task for working with a credential. The `action` closure receives a `CredentialTransaction` instance that it can perform actions on.

Warning

Don’t import UIKit in any file that imports this type. This causes ambiguity resolving the SecureElementCredential framework’s SwiftUI and UIKit symbols.

## Topics

### Configuring transactions

class Configuration

An object that provides configuration information for a transaction that the client intends to peform.

### Performing transactions

func performTransaction(using: Credential, options: CardEmulationOptions) async throws

Prompts the user for authorization and then activates a credential for card emulation.

func performTransactionInWiredMode(using: Credential, instanceAID: Data) async throws

Enters wired mode to perform a transaction.

func performCardEmulationTransactionWithCurrentCredential(options: CardEmulationOptions) async throws

Activate the current credential to perform a transaction in card emulation mode.

### Supporting types

typealias Credential

The type that represents a credential in a credential transaction.

typealias CardEmulationOptions

The type you use for card emulation options in a credential transaction.

