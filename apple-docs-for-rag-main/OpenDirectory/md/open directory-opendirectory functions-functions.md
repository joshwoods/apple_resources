

- Open Directory
-  OpenDirectory Functions 

API Collection

# OpenDirectory Functions

This document describes the functions, constants, and data types used to interact with Open Directory.

## Topics

### Working with the Open Directory Context

func ODContextGetTypeID() -> CFTypeID

Returns the type ID for the Open Directory context.

### Working with Nodes

func ODNodeCopyDetails(ODNodeRef!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

Returns a dictionary containing details about a node.

func ODNodeCopyRecord(ODNodeRef!, String!, CFString!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODRecordRef>!

Returns a reference to a record of a node.

func ODNodeCopySubnodeNames(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns the names of subnodes for a given node.

func ODNodeCopySupportedAttributes(ODNodeRef!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns an array of attribute types supported by a given node.

func ODNodeCopySupportedRecordTypes(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns an array of the record types supported by a given node.

func ODNodeCopyUnreachableSubnodeNames(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns an array of the subnodes of a given node that are currently unreachable.

func ODNodeCreateCopy(CFAllocator!, ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODNodeRef>!

Returns a copy of an existing node.

func ODNodeCreateRecord(ODNodeRef!, String!, CFString!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODRecordRef>!

Creates a record in a specified node with specified properties.

func ODNodeCreateWithName(CFAllocator!, ODSessionRef!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODNodeRef>!

Returns a new node created with a specified name.

func ODNodeCreateWithNodeType(CFAllocator!, ODSessionRef!, ODNodeType, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODNodeRef>!

Returns a new node created with a specified type.

func ODNodeCustomCall(ODNodeRef!, CFIndex, CFData!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFData!

Returns the result of a custom call to a node.

func ODNodeGetName(ODNodeRef!) -> Unmanaged&lt;CFString>!

Returns the name of a node.

func ODNodeGetTypeID() -> CFTypeID

Returns the type ID for an Open Directory node.

func ODNodeSetCredentials(ODNodeRef!, String!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets credentials for interacting with a node.

func ODNodeSetCredentialsExtended(ODNodeRef!, String!, String!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;ODContext>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets credentials for interacting with a node using a specified authentication method.

### Working with Queries

func ODQueryCopyResults(ODQueryRef!, Bool, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns results from a query synchronously.

func ODQueryCreateWithNode(CFAllocator!, ODNodeRef!, CFTypeRef!, String!, ODMatchType, CFTypeRef!, CFTypeRef!, CFIndex, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODQueryRef>!

Creates a query with a node using provided parameters.

func ODQueryCreateWithNodeType(CFAllocator!, ODNodeType, CFTypeRef!, String!, ODMatchType, CFTypeRef!, CFTypeRef!, CFIndex, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODQueryRef>!

Creates a query for a particular node type using provided parameters.

func ODQueryGetTypeID() -> CFTypeID

Returns the type ID for an Open Directory query.

func ODQueryScheduleWithRunLoop(ODQueryRef!, CFRunLoop!, CFString!)

Retrieves results from a query asynchronously by scheduling the query in a run loop.

func ODQuerySetCallback(ODQueryRef!, ODQueryCallback!, UnsafeMutableRawPointer!)

Sets the callback for an asynchronous query.

func ODQuerySetDispatchQueue(ODQueryRef!, dispatch_queue_t!)

Retrieves results from a query asynchronously by adding the query to a dispatch queue.

func ODQuerySynchronize(ODQueryRef!)

Restarts a query, disposing of any results it has obtained.

func ODQueryUnscheduleFromRunLoop(ODQueryRef!, CFRunLoop!, CFString!)

Removes a query from a specified run loop.

### Working with Records

func ODRecordAddMember(ODRecordRef!, ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Adds a record as a member of a group record.

func ODRecordAddValue(ODRecordRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Adds a value to an attribute of a record.

func ODRecordChangePassword(ODRecordRef!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Changes the password of a record.

func ODRecordContainsMember(ODRecordRef!, ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns whether a group record contains a given record.

func ODRecordCopyDetails(ODRecordRef!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

Returns the values of a record’s attributes.

func ODRecordCopyValues(ODRecordRef!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns the value of a single attribute of a record.

func ODRecordDelete(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Deletes a record from a node and invalidates the record.

func ODRecordGetRecordName(ODRecordRef!) -> Unmanaged&lt;CFString>!

Returns the official name of a record.

func ODRecordGetRecordType(ODRecordRef!) -> Unmanaged&lt;CFString>!

Returns the type of a record.

func ODRecordGetTypeID() -> CFTypeID

Returns the type ID for a record.

func ODRecordRemoveMember(ODRecordRef!, ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a record as a member from a specified group record.

func ODRecordRemoveValue(ODRecordRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a value from a record’s attribute.

func ODRecordSetNodeCredentials(ODRecordRef!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets node authentication credentials for a given record.

func ODRecordSetNodeCredentialsExtended(ODRecordRef!, String!, String!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;ODContext>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets node authentication credentials for a record using a specified authentication method.

func ODRecordSetValue(ODRecordRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets one or more attribute values of a record.

func ODRecordSynchronize(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Synchronizes a record with the directory to get current data and commit changes.

func ODRecordVerifyPassword(ODRecordRef!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Verifies a given password for a record.

func ODRecordVerifyPasswordExtended(ODRecordRef!, String!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;ODContext>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Verifies a given password for a record given a specified authentication method.

### Working with Sessions

func ODSessionCopyNodeNames(CFAllocator!, ODSessionRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns the names of nodes registered in a given session.

func ODSessionCreate(CFAllocator!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODSessionRef>!

Creates a session to be passed to node functions.

func ODSessionGetTypeID() -> CFTypeID

Returns the type ID for a session.

### Data Types

typealias ODAttributeType

An Open Directory attribute type.

typealias ODAuthenticationType

An Open Directory authentication type.

class ODContext

An Open Directory context type.

class ODNodeRef

An Open Directory node type.

class ODQueryRef

An Open Directory query type.

class ODRecordRef

An Open Directory record type.

class ODSessionRef

An Open Directory session type.

typealias ODMatchType

An Open Directory match type.

typealias ODNodeType

An Open Directory node type.

typealias ODQueryCallback

A callback function called as results from a scheduled query are returned.

typealias ODRecordType

An Open Directory record type.

\_ODAttributeType

An Open Directory attribute type.

\_ODAuthenticationType

An Open Directory authentication type.

\_ODRecordType

An Open Directory record type.

### Constants

Session Keys

Keys used when specifying session information.

Node Types

Open Directory node types.

Match Types

Types of matches used for searches.

Record Types

Types of Open Directory records.

General Attribute Types

Types of Open Directory attributes.

Configuration Attribute Types

Types of Open Directory attributes specifically for use with configure nodes.

Authentication Types

Types of authentication available in Open Directory.

### Functions

func ODNodeAddAccountPolicy(ODNodeRef!, CFDictionary!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeCopyAccountPolicies(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFDictionary!

func ODNodeCopyPolicies(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

func ODNodeCopySupportedPolicies(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

func ODNodeCustomFunction(ODNodeRef!, CFString!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFTypeRef!

func ODNodePasswordContentCheck(ODNodeRef!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeRemoveAccountPolicy(ODNodeRef!, CFDictionary!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeRemovePolicy(ODNodeRef!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeSetAccountPolicies(ODNodeRef!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeSetPolicies(ODNodeRef!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeSetPolicy(ODNodeRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordAddAccountPolicy(ODRecordRef!, CFDictionary!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordAuthenticationAllowed(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordCopyAccountPolicies(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFDictionary!

func ODRecordCopyEffectivePolicies(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

func ODRecordCopyPolicies(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

func ODRecordCopySupportedPolicies(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

func ODRecordPasswordChangeAllowed(ODRecordRef!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordRemoveAccountPolicy(ODRecordRef!, CFDictionary!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordRemovePolicy(ODRecordRef!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordSecondsUntilAuthenticationsExpire(ODRecordRef!) -> Int64

func ODRecordSecondsUntilPasswordExpires(ODRecordRef!) -> Int64

func ODRecordSetAccountPolicies(ODRecordRef!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordSetPolicies(ODRecordRef!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordSetPolicy(ODRecordRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordWillAuthenticationsExpire(ODRecordRef!, UInt64) -> Bool

func ODRecordWillPasswordExpire(ODRecordRef!, UInt64) -> Bool

## See Also

### Reference

OpenDirectory Enumerations

OpenDirectory Constants

OpenDirectory Data Types

