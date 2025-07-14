

- Authentication Services
-  ASExportedCredentialData 

Structure

# ASExportedCredentialData

A container for credential data that your app provides to an exporter or receives from an importer.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct ASExportedCredentialData
```

## Overview

This type is a wrapper object for multiple ASImportableAccount objects.

## Topics

### Creating a credential data instance

init(accounts: [ASImportableAccount])

Creates a credential data instance from an array of importable accounts.

### Accessing accounts

var accounts: [ASImportableAccount]

An array of importable accounts.

struct ASImportableAccount

An account for use in importing and exporting credentials.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Identifiable
- Sendable

## See Also

### Exporting credentials

func exportCredentials(ASExportedCredentialData) async throws

Begins the credential export process.

