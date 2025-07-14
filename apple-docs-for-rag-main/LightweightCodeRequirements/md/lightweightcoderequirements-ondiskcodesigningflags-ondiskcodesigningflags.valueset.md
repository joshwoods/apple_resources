

- LightweightCodeRequirements
- OnDiskCodeSigningFlags
-  OnDiskCodeSigningFlags.ValueSet 

Structure

# OnDiskCodeSigningFlags.ValueSet

Code signing flags that can be set on code on disk.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct ValueSet
```

## Topics

### Initializers

init(rawValue: Int64)

Creates a new option set from the given raw value.

### Instance Properties

let rawValue: Int64

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let isAdhocSigned: OnDiskCodeSigningFlags.ValueSet

The code is adhoc signed i.e. it contains a code directory and page hashes but no CMS signature.

static let isCertificateExpirationEnforced: OnDiskCodeSigningFlags.ValueSet

Flag indicating that the signature on this code should be treated as invalid if the certificate it was signed with expired.

static let isCodeSignatureRequiredForAllExecutableCode: OnDiskCodeSigningFlags.ValueSet

Flag indicating that the process should not allow code to execute from memory if that memory is not associated with a code signature.

static let isDynamicLinkerPolicyHardened: OnDiskCodeSigningFlags.ValueSet

Flag indicating that the process should get hardened dynamic linker policies.

static let isHardenedRuntimeEnforced: OnDiskCodeSigningFlags.ValueSet

Flag indicating that the process has enabled the Hardened Runtime

static let isLibraryValidationRequired: OnDiskCodeSigningFlags.ValueSet

Flag indicating that the process should enforce Library Validation.

static let isSignedByLinker: OnDiskCodeSigningFlags.ValueSet

Flag indicating that the code was signed by the linker and not an invocation of codesign.

static let signalsBusErrorOnCodeSigningFailure: OnDiskCodeSigningFlags.ValueSet

Code signing failures on page-in should be rejected as SIGBUS errors.

static let terminatesOnCodeSigningFailure: OnDiskCodeSigningFlags.ValueSet

Code signing failures on page in should cause the process to be terminated.

### Default Implementations

Equatable Implementations

OptionSet Implementations

RawRepresentable Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

