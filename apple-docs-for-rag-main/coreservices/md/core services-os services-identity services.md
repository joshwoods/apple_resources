

- Core Services
- OS Services
-  Identity Services 

API Collection

# Identity Services

Access the system's user and group database and manage access controls.

## Overview

The Core Services Identity Reference allows developers to support user and group creation, enumeration, attribute inspection, credential management as well as group membership management in their applications.

## Topics

### Classes

class CSIdentity

class CSIdentityAuthority

class CSIdentityQuery

### Functions

func CSDiskSpaceCancelRecovery(CFUUID!)

func CSDiskSpaceGetRecoveryEstimate(CFURL!) -> UInt64

func CSDiskSpaceStartRecovery(CFURL!, UInt64, CSDiskSpaceRecoveryOptions, UnsafeMutablePointer&lt;Unmanaged&lt;CFUUID>?>!, dispatch_queue_t!, CSDiskSpaceRecoveryCallback!)

func CSGetDefaultIdentityAuthority() -> Unmanaged&lt;CSIdentityAuthority>!

func CSGetLocalIdentityAuthority() -> Unmanaged&lt;CSIdentityAuthority>!

func CSGetManagedIdentityAuthority() -> Unmanaged&lt;CSIdentityAuthority>!

func CSIdentityAddAlias(CSIdentity!, CFString!)

func CSIdentityAddMember(CSIdentity!, CSIdentity!)

func CSIdentityAuthenticateUsingPassword(CSIdentity!, CFString!) -> Bool

func CSIdentityAuthorityCopyLocalizedName(CSIdentityAuthority!) -> Unmanaged&lt;CFString>!

func CSIdentityAuthorityGetTypeID() -> CFTypeID

func CSIdentityCommit(CSIdentity!, AuthorizationRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func CSIdentityCommitAsynchronously(CSIdentity!, UnsafePointer&lt;CSIdentityClientContext>!, CFRunLoop!, CFString!, AuthorizationRef!) -> Bool

func CSIdentityCreate(CFAllocator!, CSIdentityClass, CFString!, CFString!, CSIdentityFlags, CSIdentityAuthority!) -> Unmanaged&lt;CSIdentity>!

func CSIdentityCreateCopy(CFAllocator!, CSIdentity!) -> Unmanaged&lt;CSIdentity>!

func CSIdentityCreateGroupMembershipQuery(CFAllocator!, CSIdentity!) -> Unmanaged&lt;CSIdentityQuery>!

func CSIdentityCreatePersistentReference(CFAllocator!, CSIdentity!) -> Unmanaged&lt;CFData>!

func CSIdentityDelete(CSIdentity!)

func CSIdentityGetAliases(CSIdentity!) -> Unmanaged&lt;CFArray>!

func CSIdentityGetAuthority(CSIdentity!) -> Unmanaged&lt;CSIdentityAuthority>!

func CSIdentityGetCertificate(CSIdentity!) -> Unmanaged&lt;SecCertificate>!

func CSIdentityGetClass(CSIdentity!) -> CSIdentityClass

func CSIdentityGetEmailAddress(CSIdentity!) -> Unmanaged&lt;CFString>!

func CSIdentityGetFullName(CSIdentity!) -> Unmanaged&lt;CFString>!

func CSIdentityGetImageData(CSIdentity!) -> Unmanaged&lt;CFData>!

func CSIdentityGetImageDataType(CSIdentity!) -> Unmanaged&lt;CFString>!

func CSIdentityGetImageURL(CSIdentity!) -> Unmanaged&lt;CFURL>!

func CSIdentityGetPosixID(CSIdentity!) -> id_t

func CSIdentityGetPosixName(CSIdentity!) -> Unmanaged&lt;CFString>!

func CSIdentityGetTypeID() -> CFTypeID

func CSIdentityGetUUID(CSIdentity!) -> Unmanaged&lt;CFUUID>!

func CSIdentityIsCommitting(CSIdentity!) -> Bool

func CSIdentityIsEnabled(CSIdentity!) -> Bool

func CSIdentityIsHidden(CSIdentity!) -> Bool

func CSIdentityIsMemberOfGroup(CSIdentity!, CSIdentity!) -> Bool

func CSIdentityQueryCopyResults(CSIdentityQuery!) -> Unmanaged&lt;CFArray>!

func CSIdentityQueryCreate(CFAllocator!, CSIdentityClass, CSIdentityAuthority!) -> Unmanaged&lt;CSIdentityQuery>!

func CSIdentityQueryCreateForCurrentUser(CFAllocator!) -> Unmanaged&lt;CSIdentityQuery>!

func CSIdentityQueryCreateForName(CFAllocator!, CFString!, CSIdentityQueryStringComparisonMethod, CSIdentityClass, CSIdentityAuthority!) -> Unmanaged&lt;CSIdentityQuery>!

func CSIdentityQueryCreateForPersistentReference(CFAllocator!, CFData!) -> Unmanaged&lt;CSIdentityQuery>!

func CSIdentityQueryCreateForPosixID(CFAllocator!, id_t, CSIdentityClass, CSIdentityAuthority!) -> Unmanaged&lt;CSIdentityQuery>!

func CSIdentityQueryCreateForUUID(CFAllocator!, CFUUID!, CSIdentityAuthority!) -> Unmanaged&lt;CSIdentityQuery>!

func CSIdentityQueryExecute(CSIdentityQuery!, CSIdentityQueryFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func CSIdentityQueryExecuteAsynchronously(CSIdentityQuery!, CSIdentityQueryFlags, UnsafePointer&lt;CSIdentityQueryClientContext>!, CFRunLoop!, CFString!) -> Bool

func CSIdentityQueryGetTypeID() -> CFTypeID

func CSIdentityQueryStop(CSIdentityQuery!)

func CSIdentityRemoveAlias(CSIdentity!, CFString!)

func CSIdentityRemoveClient(CSIdentity!)

func CSIdentityRemoveMember(CSIdentity!, CSIdentity!)

func CSIdentitySetCertificate(CSIdentity!, SecCertificate!)

func CSIdentitySetEmailAddress(CSIdentity!, CFString!)

func CSIdentitySetFullName(CSIdentity!, CFString!)

func CSIdentitySetImageData(CSIdentity!, CFData!, CFString!)

func CSIdentitySetImageURL(CSIdentity!, CFURL!)

func CSIdentitySetIsEnabled(CSIdentity!, Bool)

func CSIdentitySetPassword(CSIdentity!, CFString!)

### Structures

struct CSIdentityClientContext

struct CSIdentityQueryClientContext

### Constants

let kCSIdentityErrorDomain: CFString!

let kCSIdentityGeneratePosixName: CFString!

