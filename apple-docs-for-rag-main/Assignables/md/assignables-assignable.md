

- Assignables
-  Assignable 

Protocol

# Assignable

Documents conforming to this protocol can be assigned to a user.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
protocol Assignable
```

## Topics

### Assigning a document

func assign(to: AnyUserIdentity) throws -> AssignedWorkDocument

Assign this document to a user.

**Required** Default implementation provided.

Deprecated

func assign(to: some UserIdentity) throws -> AssignedWorkDocument

Assign this document to a user.

**Required** Default implementation provided.

Deprecated

### Instance Methods

func makeAssignedWorkDocument() throws -> AssignedWorkDocument

Create a new instance of an AssignedWorkDocument.

**Required**

func makeAssignedWorkDocument(id: String) throws -> AssignedWorkDocument

Create a new instance of an AssignedWorkDocument.

**Required**

## Relationships

### Conforming Types

- AssignableDocument

## See Also

### Assignable document

struct AssignableDocument

An assignable document is an augmented PDF that allows teachers to mark up the PDF with the intention of students taking the assessment.

struct AssignedWorkDocument

An assigned work document is a document that contains taker and scorer markup specific to a taker. It also contains a copy of the assignable document upon which it is based.

