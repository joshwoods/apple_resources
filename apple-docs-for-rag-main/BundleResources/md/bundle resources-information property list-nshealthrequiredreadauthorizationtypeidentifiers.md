

- Bundle Resources
- Information Property List
-  NSHealthRequiredReadAuthorizationTypeIdentifiers 

Property List Key

# NSHealthRequiredReadAuthorizationTypeIdentifiers

The clinical record data types that your app must get permission to read.

iOS 12.0+iPadOS 12.0+visionOS 1.0+

## Details 

Type  

array of strings

## Discussion

Use this key to indicate that your app requires access to specific clinical record data types to function properly. Set the value to an array of strings containing the type identifiers for your required types. For a list of type identifiers, see HKClinicalTypeIdentifier.

To protect the user’s privacy, you must specify three or more required clinical record types. If the user denies authorization to any of the types, authorization fails with an HKError.Code.errorRequiredAuthorizationDenied error. Your app is not told the record types to which the user denied access.

## See Also

### Health

Setting up HealthKit

Set up and configure your HealthKit store.

NSHealthClinicalHealthRecordsShareUsageDescription

A message to the user that explains why the app requested permission to read clinical records.

**Name:** Privacy - Health Records Usage Description

NSHealthShareUsageDescription

A message to the user that explains why the app requested permission to read samples from the HealthKit store.

**Name:** Privacy - Health Share Usage Description

NSHealthUpdateUsageDescription

A message to the user that explains why the app requested permission to save samples to the HealthKit store.

**Name:** Privacy - Health Update Usage Description

