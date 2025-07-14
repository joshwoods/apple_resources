

- Security
-  Security Framework Result Codes 

API Collection

# Security Framework Result Codes

Evaluate result codes common to many Security framework functions.

## Discussion

Use the SecCopyErrorMessageString(_:_:) function to obtain a human readable string corresponding to these status codes.

In addition to the codes listed here, certain Security framework services provide additional status codes that are specific to that service. In particular, see Authorization Services Result Codes, Sessions API Result Codes, Secure Transport Result Codes, Secure Download Result Codes, and Code Signing Services Result Codes.

## Topics

### Result Strings

func SecCopyErrorMessageString(OSStatus, UnsafeMutableRawPointer?) -> CFString?

Returns a string explaining the meaning of a security result code.

### System Result Codes

var errSecSuccess: OSStatus

No error.

var errSecUnimplemented: OSStatus

A function or operation is not implemented.

var errSecDskFull: OSStatus

The disk is full.

Deprecated

var errSecDiskFull: OSStatus

The disk is full.

var errSecIO: OSStatus

I/O error.

var errSecOpWr: OSStatus

The file is already open with write permission.

var errSecParam: OSStatus

One or more parameters passed to the function are not valid.

var errSecWrPerm: OSStatus

Write permissions error.

var errSecAllocate: OSStatus

Failed to allocate memory.

var errSecUserCanceled: OSStatus

User canceled the operation.

var errSecBadReq: OSStatus

Bad parameter or invalid state for operation.

### Internal Error Result Codes

var errSecInternalComponent: OSStatus

An internal component experienced an error.

var errSecCoreFoundationUnknown: OSStatus

An unknown Core Foundation error occurred.

var errSecInternalError: OSStatus

An internal error occurred.

### Keychain Result Codes

var errSecNotAvailable: OSStatus

No trust results are available.

var errSecReadOnly: OSStatus

Read-only error.

var errSecAuthFailed: OSStatus

Authorization and/or authentication failed.

var errSecNoSuchKeychain: OSStatus

The keychain does not exist.

var errSecInvalidKeychain: OSStatus

The keychain is not valid.

var errSecDuplicateKeychain: OSStatus

A keychain with the same name already exists.

var errSecDuplicateCallback: OSStatus

More than one callback of the same name exists.

var errSecInvalidCallback: OSStatus

The callback is not valid.

var errSecDuplicateItem: OSStatus

The item already exists.

var errSecItemNotFound: OSStatus

The item cannot be found.

var errSecBufferTooSmall: OSStatus

The buffer is too small.

var errSecDataTooLarge: OSStatus

The data is too large for the particular data type.

var errSecNoSuchAttr: OSStatus

The attribute does not exist.

var errSecInvalidItemRef: OSStatus

The item reference is invalid.

var errSecInvalidSearchRef: OSStatus

The search reference is invalid.

var errSecNoSuchClass: OSStatus

The keychain item class does not exist.

var errSecNoDefaultKeychain: OSStatus

A default keychain does not exist.

var errSecInteractionNotAllowed: OSStatus

Interaction with the Security Server is not allowed.

var errSecReadOnlyAttr: OSStatus

The attribute is read-only.

var errSecWrongSecVersion: OSStatus

The version is incorrect.

var errSecKeySizeNotAllowed: OSStatus

The key size is not allowed.

var errSecNoStorageModule: OSStatus

There is no storage module available.

var errSecNoCertificateModule: OSStatus

There is no certificate module available.

var errSecNoPolicyModule: OSStatus

There is no policy module available.

var errSecInteractionRequired: OSStatus

User interaction is required.

var errSecDataNotAvailable: OSStatus

The data is not available.

var errSecDataNotModifiable: OSStatus

The data is not modifiable.

var errSecCreateChainFailed: OSStatus

The attempt to create a certificate chain failed.

var errSecInvalidPrefsDomain: OSStatus

The preference domain specified is invalid.

var errSecInDarkWake: OSStatus

The user interface cannot be displayed because the system is in a dark wake state.

### Certificate Result Codes

var errSecUnknownCriticalExtensionFlag: OSStatus

There is an unknown critical extension flag.

var errSecCertificateCannotOperate: OSStatus

The certificate cannot operate.

var errSecCertificateExpired: OSStatus

An expired certificate was detected.

var errSecCertificateNotValidYet: OSStatus

The certificate is not yet valid.

var errSecCertificateRevoked: OSStatus

The certificate was revoked.

var errSecCertificateSuspended: OSStatus

The certificate was suspended.

var errSecInvalidCertAuthority: OSStatus

The certificate authority is not valid.

var errSecInvalidCertificateGroup: OSStatus

An invalid certificate group was detected.

var errSecInvalidCertificateRef: OSStatus

An invalid certificate reference was detected.

var errSecCertificateNameNotAllowed: OSStatus

The requested name isn’t allowed for this certificate.

var errSecCertificatePolicyNotAllowed: OSStatus

The requested policy isn’t allowed for this certificate.

var errSecCertificateValidityPeriodTooLong: OSStatus

The validity period in the certificate exceeds the maximum allowed period.

### ACL Result Codes

var errSecACLAddFailed: OSStatus

An ACL add operation failed.

var errSecACLChangeFailed: OSStatus

An ACL change operation failed.

var errSecACLDeleteFailed: OSStatus

An ACL delete operation failed.

var errSecACLNotSimple: OSStatus

The access control list is not in standard simple form.

var errSecACLReplaceFailed: OSStatus

An ACL replace operation failed.

var errSecAppleAddAppACLSubject: OSStatus

Adding an application ACL subject failed.

var errSecInvalidBaseACLs: OSStatus

The base access control lists are not valid.

var errSecInvalidACL: OSStatus

An invalid access control list was detected.

### CRL Result Codes

var errSecCRLExpired: OSStatus

The certificate revocation list has expired.

var errSecCRLNotValidYet: OSStatus

The certificate revocation list is not yet valid.

var errSecCRLNotFound: OSStatus

The certificate revocation list was not found.

var errSecCRLServerDown: OSStatus

The certificate revocation list server is down.

var errSecCRLBadURI: OSStatus

The certificate revocation list has a bad uniform resource identifier.

var errSecCRLNotTrusted: OSStatus

The certificate revocation list is not trusted.

var errSecUnknownCertExtension: OSStatus

An unknown certificate extension was detected.

var errSecUnknownCRLExtension: OSStatus

An unknown certificate revocation list extension was detected.

var errSecCRLPolicyFailed: OSStatus

The certificate revocation list policy failed.

var errSecCRLAlreadySigned: OSStatus

The certificate revocation list is already signed.

var errSecIDPFailure: OSStatus

The issuing distribution point is not valid.

var errSecInvalidCRLEncoding: OSStatus

The certificate revocation list encoding is not valid.

var errSecInvalidCRLType: OSStatus

The certificate revocation list type is not valid.

var errSecInvalidCRL: OSStatus

The certificate revocation list is not valid.

var errSecInvalidCRLGroup: OSStatus

An invalid certificate revocation list group was detected.

var errSecInvalidCRLIndex: OSStatus

The certificate revocation list index is not valid.

var errSecInvaldCRLAuthority: OSStatus

The certificate revocation list authority is not valid.

Deprecated

### SMIME Result Codes

var errSecSMIMEEmailAddressesNotFound: OSStatus

An email address mismatch was detected.

var errSecSMIMEBadExtendedKeyUsage: OSStatus

The appropriate extended key usage for SMIME is not found.

var errSecSMIMEBadKeyUsage: OSStatus

The key usage is not compatible with SMIME.

var errSecSMIMEKeyUsageNotCritical: OSStatus

The key usage extension is not marked as critical.

var errSecSMIMENoEmailAddress: OSStatus

No email address is found in the certificate.

var errSecSMIMESubjAltNameNotCritical: OSStatus

The subject alternative name extension is not marked as critical.

var errSecSSLBadExtendedKeyUsage: OSStatus

The appropriate extended key usage for SSL is not found.

### OCSP Result Codes

var errSecOCSPBadResponse: OSStatus

The online certificate status protocol (OCSP) response is incorrect or cannot be parsed.

var errSecOCSPBadRequest: OSStatus

The online certificate status protocol (OCSP) request is incorrect or cannot be parsed.

var errSecOCSPUnavailable: OSStatus

The online certificate status protocol (OCSP) service is unavailable.

var errSecOCSPStatusUnrecognized: OSStatus

The online certificate status protocol (OCSP) server does not recognize this certificate.

var errSecEndOfData: OSStatus

An end-of-data was detected.

var errSecIncompleteCertRevocationCheck: OSStatus

An incomplete certificate revocation check occurred.

var errSecNetworkFailure: OSStatus

A network failure occurred.

var errSecOCSPNotTrustedToAnchor: OSStatus

The online certificate status protocol (OCSP) response is not trusted to a root or anchor certificate.

var errSecRecordModified: OSStatus

The record is modified.

var errSecOCSPSignatureError: OSStatus

The online certificate status protocol (OCSP) response has an invalid signature.

var errSecOCSPNoSigner: OSStatus

The online certificate status protocol (OCSP) response has no signer.

var errSecOCSPResponderMalformedReq: OSStatus

The online certificate status protocol (OCSP) responder detected a malformed request.

var errSecOCSPResponderInternalError: OSStatus

The online certificate status protocol (OCSP) responder detected an internal error.

var errSecOCSPResponderTryLater: OSStatus

The online certificate status protocol (OCSP) responder is busy, try again later.

var errSecOCSPResponderSignatureRequired: OSStatus

The online certificate status protocol (OCSP) responder requires a signature.

var errSecOCSPResponderUnauthorized: OSStatus

The online certificate status protocol (OCSP) responder rejects the request as unauthorized.

var errSecOCSPResponseNonceMismatch: OSStatus

The online certificate status protocol (OCSP) response nonce does not match the request.

### Code Signing Result Codes

var errSecCodeSigningBadCertChainLength: OSStatus

Code signing encountered an incorrect certificate chain length.

var errSecCodeSigningNoBasicConstraints: OSStatus

Code signing found no basic constraints.

var errSecCodeSigningBadPathLengthConstraint: OSStatus

Code signing encountered an incorrect path length constraint.

var errSecCodeSigningNoExtendedKeyUsage: OSStatus

Code signing found no extended key usage.

var errSecCodeSigningDevelopment: OSStatus

Code signing indicated use of a development-only certificate.

var errSecResourceSignBadCertChainLength: OSStatus

Resource signing detects an incorrect certificate chain length.

var errSecResourceSignBadExtKeyUsage: OSStatus

Resource signing detects an error in the extended key usage.

var errSecTrustSettingDeny: OSStatus

The trust setting for this policy is set to Deny.

var errSecInvalidSubjectName: OSStatus

An invalid certificate subject name was detected.

var errSecUnknownQualifiedCertStatement: OSStatus

An unknown qualified certificate statement was detected.

### Mobile Me Result Codes

var errSecMobileMeRequestQueued: OSStatus

The MobileMe request will be sent during the next connection.

var errSecMobileMeRequestRedirected: OSStatus

The MobileMe request was redirected.

var errSecMobileMeServerError: OSStatus

A MobileMe server error occurred.

var errSecMobileMeServerNotAvailable: OSStatus

The MobileMe server is not available.

var errSecMobileMeServerAlreadyExists: OSStatus

The MobileMe server reported that the item already exists.

var errSecMobileMeServerServiceErr: OSStatus

A MobileMe service error occurred.

var errSecMobileMeRequestAlreadyPending: OSStatus

A MobileMe request is already pending.

var errSecMobileMeNoRequestPending: OSStatus

MobileMe has no request pending.

var errSecMobileMeCSRVerifyFailure: OSStatus

A MobileMe certificate signing request verification failure occurred.

var errSecMobileMeFailedConsistencyCheck: OSStatus

MobileMe found a failed consistency check.

### Cryptographic Key Result Codes

var errSecKeyUsageIncorrect: OSStatus

The key usage is incorrect.

var errSecKeyBlobTypeIncorrect: OSStatus

The key blob type is incorrect.

var errSecKeyHeaderInconsistent: OSStatus

The key header is inconsistent.

var errSecKeyIsSensitive: OSStatus

The key must be wrapped to be exported.

var errSecUnsupportedKeyFormat: OSStatus

The key header format is not supported.

var errSecUnsupportedKeySize: OSStatus

The key size is not supported.

var errSecInvalidKeyUsageMask: OSStatus

The key usage mask is not valid.

var errSecUnsupportedKeyUsageMask: OSStatus

The key usage mask is not supported.

var errSecInvalidKeyAttributeMask: OSStatus

The key attribute mask is not valid.

var errSecUnsupportedKeyAttributeMask: OSStatus

The key attribute mask is not supported.

var errSecInvalidKeyLabel: OSStatus

The key label is not valid.

var errSecUnsupportedKeyLabel: OSStatus

The key label is not supported.

var errSecInvalidKeyFormat: OSStatus

The key format is not valid.

var errSecInvalidKeyBlob: OSStatus

The specified database has an invalid key blob.

var errSecInvalidKeyHierarchy: OSStatus

An invalid key hierarchy was detected.

var errSecInvalidKeyRef: OSStatus

An invalid key was encountered.

var errSecInvalidKeyUsageForPolicy: OSStatus

The key usage is not valid for the specified policy.

### Invalid Attribute Result Codes

var errSecInvalidAttributeKey: OSStatus

A key attribute is not valid.

var errSecInvalidAttributeInitVector: OSStatus

An init vector attribute is not valid.

var errSecInvalidAttributeSalt: OSStatus

A salt attribute is not valid.

var errSecInvalidAttributePadding: OSStatus

A padding attribute is not valid.

var errSecInvalidAttributeRandom: OSStatus

A random number attribute is not valid.

var errSecInvalidAttributeSeed: OSStatus

A seed attribute is not valid.

var errSecInvalidAttributePassphrase: OSStatus

A passphrase attribute is not valid.

var errSecInvalidAttributeKeyLength: OSStatus

A key length attribute is not valid.

var errSecInvalidAttributeBlockSize: OSStatus

A block size attribute is not valid.

var errSecInvalidAttributeOutputSize: OSStatus

An output size attribute is not valid.

var errSecInvalidAttributeRounds: OSStatus

The number of rounds attribute is not valid.

var errSecInvalidAlgorithmParms: OSStatus

An algorithm parameters attribute is not valid.

var errSecInvalidAttributeLabel: OSStatus

A label attribute is not valid.

var errSecInvalidAttributeKeyType: OSStatus

A key type attribute is not valid.

var errSecInvalidAttributeMode: OSStatus

A mode attribute is not valid.

var errSecInvalidAttributeEffectiveBits: OSStatus

An effective bits attribute is not valid.

var errSecInvalidAttributeStartDate: OSStatus

A start date attribute is not valid.

var errSecInvalidAttributeEndDate: OSStatus

An end date attribute is not valid.

var errSecInvalidAttributeVersion: OSStatus

A version attribute is not valid.

var errSecInvalidAttributePrime: OSStatus

A prime attribute is not valid.

var errSecInvalidAttributeBase: OSStatus

A base attribute is not valid.

var errSecInvalidAttributeSubprime: OSStatus

A subprime attribute is not valid.

var errSecInvalidAttributeIterationCount: OSStatus

An iteration count attribute is not valid.

var errSecInvalidAttributeDLDBHandle: OSStatus

A database handle attribute is not valid.

var errSecInvalidAttributeAccessCredentials: OSStatus

An access credentials attribute is not valid.

var errSecInvalidAttributePublicKeyFormat: OSStatus

A public key format attribute is not valid.

var errSecInvalidAttributePrivateKeyFormat: OSStatus

A private key format attribute is not valid.

var errSecInvalidAttributeSymmetricKeyFormat: OSStatus

A symmetric key format attribute is not valid.

var errSecInvalidAttributeWrappedKeyFormat: OSStatus

A wrapped key format attribute is not valid.

### Missing Attribute Result Codes

var errSecMissingAttributeKey: OSStatus

A key attribute is missing.

var errSecMissingAttributeInitVector: OSStatus

An init vector attribute is missing.

var errSecMissingAttributeSalt: OSStatus

A salt attribute is missing.

var errSecMissingAttributePadding: OSStatus

A padding attribute is missing.

var errSecMissingAttributeRandom: OSStatus

A random number attribute is missing.

var errSecMissingAttributeSeed: OSStatus

A seed attribute is missing.

var errSecMissingAttributePassphrase: OSStatus

A passphrase attribute is missing.

var errSecMissingAttributeKeyLength: OSStatus

A key length attribute is missing.

var errSecMissingAttributeBlockSize: OSStatus

A block size attribute is missing.

var errSecMissingAttributeOutputSize: OSStatus

An output size attribute is missing.

var errSecMissingAttributeRounds: OSStatus

The number of rounds attribute is missing.

var errSecMissingAlgorithmParms: OSStatus

An algorithm parameters attribute is missing.

var errSecMissingAttributeLabel: OSStatus

A label attribute is missing.

var errSecMissingAttributeKeyType: OSStatus

A key type attribute is missing.

var errSecMissingAttributeMode: OSStatus

A mode attribute is missing.

var errSecMissingAttributeEffectiveBits: OSStatus

An effective bits attribute is missing.

var errSecMissingAttributeStartDate: OSStatus

A start date attribute is missing.

var errSecMissingAttributeEndDate: OSStatus

An end date attribute is missing.

var errSecMissingAttributeVersion: OSStatus

A version attribute is missing.

var errSecMissingAttributePrime: OSStatus

A prime attribute is missing.

var errSecMissingAttributeBase: OSStatus

A base attribute is missing.

var errSecMissingAttributeSubprime: OSStatus

A subprime attribute is missing.

var errSecMissingAttributeIterationCount: OSStatus

An iteration count attribute is missing.

var errSecMissingAttributeDLDBHandle: OSStatus

A database handle attribute is missing.

var errSecMissingAttributeAccessCredentials: OSStatus

An access credentials attribute is missing.

var errSecMissingAttributePublicKeyFormat: OSStatus

A public key format attribute is missing.

var errSecMissingAttributePrivateKeyFormat: OSStatus

A private key format attribute is missing.

var errSecMissingAttributeSymmetricKeyFormat: OSStatus

A symmetric key format attribute is missing.

var errSecMissingAttributeWrappedKeyFormat: OSStatus

A wrapped key format attribute is missing.

### Timestamp Result Codes

var errSecTimestampMissing: OSStatus

A timestamp is expected but is not found.

var errSecTimestampInvalid: OSStatus

The timestamp is not valid.

var errSecTimestampNotTrusted: OSStatus

The timestamp is not trusted.

var errSecTimestampServiceNotAvailable: OSStatus

var errSecTimestampBadAlg: OSStatus

Found an unrecognized or unsupported algorithm identifier (AI) in timestamp.

var errSecTimestampBadRequest: OSStatus

The timestamp transaction is not permitted or supported.

var errSecTimestampBadDataFormat: OSStatus

The timestamp data submitted has the wrong format.

var errSecTimestampTimeNotAvailable: OSStatus

The time source for the timestamp authority is not available.

var errSecTimestampUnacceptedPolicy: OSStatus

The requested policy is not supported by the timestamp authority.

var errSecTimestampUnacceptedExtension: OSStatus

The requested extension is not supported by the timestamp authority.

var errSecTimestampAddInfoNotAvailable: OSStatus

The additional information requested is not available.

var errSecTimestampSystemFailure: OSStatus

The timestamp request cannot be handled due to a system failure.

var errSecSigningTimeMissing: OSStatus

A signing time is missing.

var errSecTimestampRejection: OSStatus

A timestamp transaction is rejected.

var errSecTimestampWaiting: OSStatus

A timestamp transaction is waiting.

var errSecTimestampRevocationWarning: OSStatus

A timestamp authority revocation warning is issued.

var errSecTimestampRevocationNotification: OSStatus

A timestamp authority revocation notification is issued.

### Invalid parameter result codes

var errSecInvalidAction: OSStatus

The action is invalid.

var errSecInvalidAddinFunctionTable: OSStatus

An invalid add-in function table was detected.

var errSecInvalidAlgorithm: OSStatus

An invalid algorithm was detected.

var errSecInvalidAuthority: OSStatus

The authority is not valid.

var errSecInvalidAuthorityKeyID: OSStatus

The authority key ID is not valid.

var errSecInvalidBundleInfo: OSStatus

The bundle information is not valid.

var errSecInvalidContext: OSStatus

An invalid context was detected.

var errSecInvalidDBList: OSStatus

An invalid DB list was detected.

var errSecInvalidDBLocation: OSStatus

The database location is not valid.

var errSecInvalidData: OSStatus

Invalid data was detected.

var errSecInvalidDatabaseBlob: OSStatus

The specified database has an invalid blob.

var errSecInvalidDigestAlgorithm: OSStatus

An invalid digest algorithm was detected.

var errSecInvalidEncoding: OSStatus

The encoding is not valid.

var errSecInvalidExtendedKeyUsage: OSStatus

The extended key usage is not valid.

var errSecInvalidFormType: OSStatus

The form type is not valid.

var errSecInvalidGUID: OSStatus

An invalid GUID was detected.

var errSecInvalidHandle: OSStatus

An invalid handle was encountered.

var errSecInvalidHandleUsage: OSStatus

The common security services manager handle does not match with the service type.

var errSecInvalidID: OSStatus

The ID is not valid.

var errSecInvalidIDLinkage: OSStatus

The ID linkage is not valid.

var errSecInvalidIdentifier: OSStatus

The identifier is not valid.

var errSecInvalidIndex: OSStatus

The index is not valid.

var errSecInvalidIndexInfo: OSStatus

The index information is not valid.

var errSecInvalidInputVector: OSStatus

The input vector is not valid.

var errSecInvalidLoginName: OSStatus

An invalid login name was detected.

var errSecInvalidModifyMode: OSStatus

The modify mode is not valid.

var errSecInvalidName: OSStatus

An invalid name was detected.

var errSecInvalidNetworkAddress: OSStatus

An invalid network address was detected.

var errSecInvalidNewOwner: OSStatus

The new owner is not valid.

var errSecInvalidNumberOfFields: OSStatus

An invalid number of fields were detected.

var errSecInvalidOutputVector: OSStatus

The output vector is not valid.

var errSecInvalidOwnerEdit: OSStatus

An invalid attempt to change the owner of an item.

var errSecInvalidPVC: OSStatus

An invalid pointer validation checking policy was detected.

var errSecInvalidParsingModule: OSStatus

The parsing module is not valid.

var errSecInvalidPassthroughID: OSStatus

An invalid passthrough ID was detected.

var errSecInvalidPasswordRef: OSStatus

The password reference is invalid.

var errSecInvalidPointer: OSStatus

An invalid pointer was detected.

var errSecInvalidPolicyIdentifiers: OSStatus

The policy identifiers are not valid.

var errSecInvalidQuery: OSStatus

The specified query is not valid.

var errSecInvalidReason: OSStatus

The trust policy reason is not valid.

var errSecInvalidRecord: OSStatus

An invalid record was detected.

var errSecInvalidRequestInputs: OSStatus

The request inputs are not valid.

var errSecInvalidRequestor: OSStatus

The requestor is not valid.

var errSecInvalidResponseVector: OSStatus

The response vector is not valid.

var errSecInvalidRoot: OSStatus

The root or anchor certificate is not valid.

var errSecInvalidSampleValue: OSStatus

An invalid sample value was detected.

var errSecInvalidScope: OSStatus

An invalid scope was detected.

var errSecInvalidServiceMask: OSStatus

An invalid service mask was detected.

var errSecInvalidSignature: OSStatus

An invalid signature was detected.

var errSecInvalidStopOnPolicy: OSStatus

The stop-on policy is not valid.

var errSecInvalidSubServiceID: OSStatus

An invalid sub-service ID was detected.

var errSecInvalidSubjectKeyID: OSStatus

The subject key ID is not valid.

var errSecInvalidTimeString: OSStatus

The time specified is not valid.

var errSecInvalidTrustSetting: OSStatus

The trust setting is invalid.

var errSecInvalidTrustSettings: OSStatus

The trust settings record is corrupted.

var errSecInvalidTuple: OSStatus

The tuple is not valid.

var errSecInvalidTupleCredendtials: OSStatus

The tuple credentials are not valid.

Deprecated

var errSecInvalidTupleGroup: OSStatus

The tuple group is not valid.

var errSecInvalidValidityPeriod: OSStatus

The validity period is not valid.

var errSecInvalidValue: OSStatus

An invalid value was detected.

### Unsupported input result codes

var errSecUnsupportedAddressType: OSStatus

The address type is not supported.

var errSecUnsupportedFieldFormat: OSStatus

The field format is not supported.

var errSecUnsupportedFormat: OSStatus

The specified import or export format is not supported.

var errSecUnsupportedIndexInfo: OSStatus

The index information is not supported.

var errSecUnsupportedLocality: OSStatus

The locality is not supported.

var errSecUnsupportedNumAttributes: OSStatus

The number of attributes is not supported.

var errSecUnsupportedNumIndexes: OSStatus

The number of indexes is not supported.

var errSecUnsupportedNumRecordTypes: OSStatus

The number of record types is not supported.

var errSecUnsupportedNumSelectionPreds: OSStatus

The number of selection predicates is not supported.

var errSecUnsupportedOperator: OSStatus

The operator is not supported.

var errSecUnsupportedQueryLimits: OSStatus

The query limits are not supported.

var errSecUnsupportedService: OSStatus

The service is not supported.

var errSecUnsupportedVectorOfBuffers: OSStatus

The vector of buffers is not supported.

### Apple specific result codes

var errSecAppleInvalidKeyEndDate: OSStatus

The specified key has an invalid end date.

var errSecAppleInvalidKeyStartDate: OSStatus

The specified key has an invalid start date.

var errSecApplePublicKeyIncomplete: OSStatus

The public key is incomplete.

var errSecAppleSSLv2Rollback: OSStatus

A SSLv2 rollback error has occurred.

var errSecAppleSignatureMismatch: OSStatus

A signature mismatch has occurred.

### Module manager result codes

var errSecEMMLoadFailed: OSStatus

The elective module manager load failed.

var errSecEMMUnloadFailed: OSStatus

The elective module manager unload has failed.

var errSecModuleManagerInitializeFailed: OSStatus

A module failed to initialize.

var errSecModuleManagerNotFound: OSStatus

A module was not found.

var errSecModuleManifestVerifyFailed: OSStatus

A module manifest verification failure occurred.

var errSecModuleNotLoaded: OSStatus

A module was not loaded.

### Other Result Codes

var errSecAddinLoadFailed: OSStatus

The add-in load operation failed.

var errSecAddinUnloadFailed: OSStatus

The add-in unload operation failed.

var errSecAlgorithmMismatch: OSStatus

An algorithm mismatch occurred.

var errSecAlreadyLoggedIn: OSStatus

The user is already logged in.

var errSecAttachHandleBusy: OSStatus

The CSP handle was busy.

var errSecAttributeNotInContext: OSStatus

An attribute was not in the context.

var errSecBlockSizeMismatch: OSStatus

A block size mismatch occurred.

var errSecCallbackFailed: OSStatus

A callback failed.

var errSecConversionError: OSStatus

A conversion error has occurred.

var errSecDatabaseLocked: OSStatus

The database is locked.

var errSecDatastoreIsOpen: OSStatus

The data store is open.

var errSecDecode: OSStatus

Unable to decode the provided data.

var errSecDeviceError: OSStatus

A device error was encountered.

var errSecDeviceFailed: OSStatus

A device failure has occurred.

var errSecDeviceReset: OSStatus

A device reset has occurred.

var errSecDeviceVerifyFailed: OSStatus

A device verification failure has occurred.

var errSecEventNotificationCallbackNotFound: OSStatus

An event notification callback was not found.

var errSecExtendedKeyUsageNotCritical: OSStatus

The extended key usage extension was not marked critical.

var errSecFieldSpecifiedMultiple: OSStatus

Too many fields were specified.

var errSecFileTooBig: OSStatus

The file is too big.

var errSecFunctionFailed: OSStatus

A function has failed.

var errSecFunctionIntegrityFail: OSStatus

A function address is not within the verified module.

var errSecHostNameMismatch: OSStatus

A host name mismatch has occurred.

var errSecIncompatibleDatabaseBlob: OSStatus

The specified database has an incompatible blob.

var errSecIncompatibleFieldFormat: OSStatus

The field format is incompatible.

var errSecIncompatibleKeyBlob: OSStatus

The specified database has an incompatible key blob.

var errSecIncompatibleVersion: OSStatus

The version is incompatible.

var errSecInputLengthError: OSStatus

An input length error occurred.

var errSecInsufficientClientID: OSStatus

The client ID is incorrect.

var errSecInsufficientCredentials: OSStatus

Insufficient credentials were detected.

var errSecInvalidAccessCredentials: OSStatus

Invalid access credentials were detected.

var errSecInvalidAccessRequest: OSStatus

The access request is invalid.

var errSecLibraryReferenceNotFound: OSStatus

A library reference was not found.

var errSecMDSError: OSStatus

A module directory service error occurred.

var errSecMemoryError: OSStatus

A memory error occurred.

var errSecMissingEntitlement: OSStatus

A required entitlement is missing.

var errSecMissingRequiredExtension: OSStatus

A required certificate extension is missing.

var errSecMissingValue: OSStatus

A missing value was detected.

var errSecMultiplePrivKeys: OSStatus

An attempt was made to import multiple private keys.

var errSecMultipleValuesUnsupported: OSStatus

Multiple values are not supported.

var errSecNoAccessForItem: OSStatus

The specified item has no access control.

var errSecNoBasicConstraints: OSStatus

No basic constraints were found.

var errSecNoBasicConstraintsCA: OSStatus

No basic CA constraints were found.

var errSecNoDefaultAuthority: OSStatus

No default authority was detected.

var errSecNoFieldValues: OSStatus

No field values were detected.

var errSecNoTrustSettings: OSStatus

No trust settings were found.

var errSecNotInitialized: OSStatus

A function was called without initializing the common security services manager.

var errSecNotLoggedIn: OSStatus

You are not logged in.

var errSecNotSigner: OSStatus

The certificate is not signed by its proposed parent.

var errSecNotTrusted: OSStatus

The trust policy is not trusted.

var errSecOutputLengthError: OSStatus

An output length error was detected.

var errSecPVCAlreadyConfigured: OSStatus

The PVC is already configured.

var errSecPVCReferentNotFound: OSStatus

A reference to the calling module was not found in the list of authorized callers.

var errSecPassphraseRequired: OSStatus

A password is required for import or export.

var errSecPathLengthConstraintExceeded: OSStatus

The path length constraint was exceeded.

var errSecPkcs12VerifyFailure: OSStatus

MAC verification failed during PKCS12 Import.

var errSecPolicyNotFound: OSStatus

The specified policy cannot be found.

var errSecPrivilegeNotGranted: OSStatus

The privilege is not granted.

var errSecPrivilegeNotSupported: OSStatus

The privilege is not supported.

var errSecPublicKeyInconsistent: OSStatus

The public key is inconsistent.

var errSecQuerySizeUnknown: OSStatus

The query size is unknown.

var errSecQuotaExceeded: OSStatus

The quota was exceeded.

var errSecRejectedForm: OSStatus

The trust policy has a rejected form.

var errSecRequestDescriptor: OSStatus

The request descriptor is not valid.

var errSecRequestLost: OSStatus

The request is lost.

var errSecRequestRejected: OSStatus

The request is rejected.

var errSecSelfCheckFailed: OSStatus

Self-check failed.

var errSecServiceNotAvailable: OSStatus

Self-check failed.

var errSecStagedOperationInProgress: OSStatus

A staged operation is in progress.

var errSecStagedOperationNotStarted: OSStatus

A staged operation was not started.

var errSecTagNotFound: OSStatus

The specified tag is not found.

var errSecTrustNotAvailable: OSStatus

No trust results are available.

var errSecUnknownFormat: OSStatus

The item you are trying to import has an unknown format.

var errSecUnknownTag: OSStatus

An unknown tag was detected.

var errSecVerificationFailure: OSStatus

A verification failure occurred.

var errSecVerifyActionFailed: OSStatus

A verify action failed.

var errSecVerifyFailed: OSStatus

A cryptographic verification failure occurred.

## See Also

### Related Documentation

Sessions API Result Codes

Recognize result codes specific to the sessions API.

Secure Transport Result Codes

Recognize result codes specific to the secure transport API.

Code Signing Services Result Codes

Recognize result codes specific to the code signing services API.

