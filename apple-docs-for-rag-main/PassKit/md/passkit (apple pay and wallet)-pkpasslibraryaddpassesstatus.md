

- PassKit (Apple Pay and Wallet)
-  PKPassLibraryAddPassesStatus 

Enumeration

# PKPassLibraryAddPassesStatus

Statuses that PassKit uses when it adds passes to the pass library.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 3.0+

``` source
enum PKPassLibraryAddPassesStatus
```

## Topics

### Constants

case didAddPasses

A status that occurs when the user successfully adds one or more passes.

case shouldReviewPasses

A status that occurs when the app prompts the user to review the passes.

case didCancelAddPasses

A status that occurs when the user cancels the addition of passes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Adding passes

func canAddSecureElementPass(primaryAccountIdentifier: String) -> Bool

Returns a Boolean value that indicates whether PassKit can add a Secure Element pass for the specified account.

func canAddFelicaPass() -> Bool

Returns a Boolean value that indicates whether the library can add FeliCa™ passes.

func addPasses([PKPass], withCompletionHandler: ((PKPassLibraryAddPassesStatus) -> Void)?)

Presents a user interface for adding multiple passes at once.

