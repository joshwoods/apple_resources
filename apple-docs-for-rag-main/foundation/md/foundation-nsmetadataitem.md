

- Foundation
-  NSMetadataItem 

Class

# NSMetadataItem

The metadata associated with a file.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMetadataItem
```

## Overview

Metadata items provide a simple interface to retrieve the available attribute names and values.

## Topics

### Creating a Metadata Item

init?(url: URL)

Initializes a metadata item with a given URL.

### Getting Item Attributes

var attributes: [String]

An array containing the attribute keys for the metadata item’s values.

func value(forAttribute: String) -> Any?

Returns the receiver’s metadata attribute name specified by a given key.

func values(forAttributes: [String]) -> [String : Any]?

Returns a dictionary containing the key-value pairs for the attribute names specified by a given array of keys.

### Item Attribute Keys

let NSMetadataItemAudiencesKey: String

let NSMetadataItemAudioBitRateKey: String

let NSMetadataItemAudioChannelCountKey: String

let NSMetadataItemAudioEncodingApplicationKey: String

let NSMetadataItemAudioSampleRateKey: String

let NSMetadataItemAudioTrackNumberKey: String

let NSMetadataItemAuthorAddressesKey: String

let NSMetadataItemAuthorEmailAddressesKey: String

let NSMetadataItemAuthorsKey: String

let NSMetadataItemAcquisitionMakeKey: String

let NSMetadataItemAcquisitionModelKey: String

let NSMetadataItemAlbumKey: String

let NSMetadataItemAltitudeKey: String

let NSMetadataItemApertureKey: String

let NSMetadataItemAppleLoopDescriptorsKey: String

let NSMetadataItemAppleLoopsKeyFilterTypeKey: String

let NSMetadataItemAppleLoopsLoopModeKey: String

let NSMetadataItemAppleLoopsRootKeyKey: String

let NSMetadataItemApplicationCategoriesKey: String

let NSMetadataItemAttributeChangeDateKey: String

let NSMetadataItemFSNameKey: String

let NSMetadataItemDisplayNameKey: String

let NSMetadataItemURLKey: String

let NSMetadataItemPathKey: String

let NSMetadataItemFSSizeKey: String

let NSMetadataItemFSCreationDateKey: String

let NSMetadataItemFSContentChangeDateKey: String

let NSMetadataItemBitsPerSampleKey: String

let NSMetadataItemCFBundleIdentifierKey: String

let NSMetadataItemCameraOwnerKey: String

let NSMetadataItemCityKey: String

let NSMetadataItemCodecsKey: String

let NSMetadataItemColorSpaceKey: String

let NSMetadataItemCommentKey: String

let NSMetadataItemComposerKey: String

let NSMetadataItemContactKeywordsKey: String

let NSMetadataItemContentCreationDateKey: String

let NSMetadataItemContentModificationDateKey: String

let NSMetadataItemContentTypeKey: String

let NSMetadataItemContentTypeTreeKey: String

let NSMetadataItemContributorsKey: String

let NSMetadataItemCopyrightKey: String

let NSMetadataItemCountryKey: String

let NSMetadataItemCoverageKey: String

let NSMetadataItemCreatorKey: String

let NSMetadataItemDateAddedKey: String

let NSMetadataItemDeliveryTypeKey: String

let NSMetadataItemDescriptionKey: String

let NSMetadataItemDirectorKey: String

let NSMetadataItemDownloadedDateKey: String

let NSMetadataItemDueDateKey: String

let NSMetadataItemDurationSecondsKey: String

let NSMetadataItemEXIFGPSVersionKey: String

let NSMetadataItemEXIFVersionKey: String

let NSMetadataItemEditorsKey: String

let NSMetadataItemEmailAddressesKey: String

let NSMetadataItemEncodingApplicationsKey: String

let NSMetadataItemExecutableArchitecturesKey: String

let NSMetadataItemExecutablePlatformKey: String

let NSMetadataItemExposureModeKey: String

let NSMetadataItemExposureProgramKey: String

let NSMetadataItemExposureTimeSecondsKey: String

let NSMetadataItemExposureTimeStringKey: String

let NSMetadataItemFNumberKey: String

let NSMetadataItemFinderCommentKey: String

let NSMetadataItemFlashOnOffKey: String

let NSMetadataItemFocalLength35mmKey: String

let NSMetadataItemFocalLengthKey: String

let NSMetadataItemFontsKey: String

let NSMetadataItemGPSAreaInformationKey: String

let NSMetadataItemGPSDOPKey: String

let NSMetadataItemGPSDateStampKey: String

let NSMetadataItemGPSDestBearingKey: String

let NSMetadataItemGPSDestDistanceKey: String

let NSMetadataItemGPSDestLatitudeKey: String

let NSMetadataItemGPSDestLongitudeKey: String

let NSMetadataItemGPSDifferentalKey: String

let NSMetadataItemGPSMapDatumKey: String

let NSMetadataItemGPSMeasureModeKey: String

let NSMetadataItemGPSProcessingMethodKey: String

let NSMetadataItemGPSStatusKey: String

let NSMetadataItemGPSTrackKey: String

let NSMetadataItemGenreKey: String

let NSMetadataItemHasAlphaChannelKey: String

let NSMetadataItemHeadlineKey: String

let NSMetadataItemISOSpeedKey: String

let NSMetadataItemIdentifierKey: String

let NSMetadataItemImageDirectionKey: String

let NSMetadataItemInformationKey: String

let NSMetadataItemInstantMessageAddressesKey: String

let NSMetadataItemInstructionsKey: String

let NSMetadataItemIsApplicationManagedKey: String

let NSMetadataItemIsGeneralMIDISequenceKey: String

let NSMetadataItemIsLikelyJunkKey: String

let NSMetadataItemKeySignatureKey: String

let NSMetadataItemKeywordsKey: String

let NSMetadataItemKindKey: String

let NSMetadataItemLanguagesKey: String

let NSMetadataItemLastUsedDateKey: String

let NSMetadataItemLatitudeKey: String

let NSMetadataItemLayerNamesKey: String

let NSMetadataItemLensModelKey: String

let NSMetadataItemLongitudeKey: String

let NSMetadataItemLyricistKey: String

let NSMetadataItemMaxApertureKey: String

let NSMetadataItemMediaTypesKey: String

let NSMetadataItemMeteringModeKey: String

let NSMetadataItemMusicalGenreKey: String

let NSMetadataItemMusicalInstrumentCategoryKey: String

let NSMetadataItemMusicalInstrumentNameKey: String

let NSMetadataItemNamedLocationKey: String

let NSMetadataItemNumberOfPagesKey: String

let NSMetadataItemOrganizationsKey: String

let NSMetadataItemOrientationKey: String

let NSMetadataItemOriginalFormatKey: String

let NSMetadataItemOriginalSourceKey: String

let NSMetadataItemPageHeightKey: String

let NSMetadataItemPageWidthKey: String

let NSMetadataItemParticipantsKey: String

let NSMetadataItemPerformersKey: String

let NSMetadataItemPhoneNumbersKey: String

let NSMetadataItemPixelCountKey: String

let NSMetadataItemPixelHeightKey: String

let NSMetadataItemPixelWidthKey: String

let NSMetadataItemProducerKey: String

let NSMetadataItemProfileNameKey: String

let NSMetadataItemProjectsKey: String

let NSMetadataItemPublishersKey: String

let NSMetadataItemRecipientAddressesKey: String

let NSMetadataItemRecipientEmailAddressesKey: String

let NSMetadataItemRecipientsKey: String

let NSMetadataItemRecordingDateKey: String

let NSMetadataItemRecordingYearKey: String

let NSMetadataItemRedEyeOnOffKey: String

let NSMetadataItemResolutionHeightDPIKey: String

let NSMetadataItemResolutionWidthDPIKey: String

let NSMetadataItemRightsKey: String

let NSMetadataItemSecurityMethodKey: String

let NSMetadataItemSpeedKey: String

let NSMetadataItemStarRatingKey: String

let NSMetadataItemStateOrProvinceKey: String

let NSMetadataItemStreamableKey: String

let NSMetadataItemSubjectKey: String

let NSMetadataItemTempoKey: String

let NSMetadataItemTextContentKey: String

let NSMetadataItemThemeKey: String

let NSMetadataItemTimeSignatureKey: String

let NSMetadataItemTimestampKey: String

let NSMetadataItemTitleKey: String

let NSMetadataItemTotalBitRateKey: String

let NSMetadataItemVersionKey: String

let NSMetadataItemVideoBitRateKey: String

let NSMetadataItemWhereFromsKey: String

let NSMetadataItemWhiteBalanceKey: String

### iCloud Keys

Attribute keys that describe cloud-related information about the item.

let NSMetadataItemIsUbiquitousKey: String

let NSMetadataUbiquitousItemContainerDisplayNameKey: String

let NSMetadataUbiquitousItemDownloadRequestedKey: String

let NSMetadataUbiquitousItemIsExternalDocumentKey: String

let NSMetadataUbiquitousItemURLInLocalContainerKey: String

let NSMetadataUbiquitousItemHasUnresolvedConflictsKey: String

let NSMetadataUbiquitousItemIsDownloadedKey: StringDeprecated

let NSMetadataUbiquitousItemIsDownloadingKey: String

let NSMetadataUbiquitousItemIsUploadedKey: String

let NSMetadataUbiquitousItemIsUploadingKey: String

let NSMetadataUbiquitousItemPercentDownloadedKey: String

let NSMetadataUbiquitousItemPercentUploadedKey: String

let NSMetadataUbiquitousItemDownloadingStatusKey: String

let NSMetadataUbiquitousItemDownloadingErrorKey: String

let NSMetadataUbiquitousItemUploadingErrorKey: String

let NSMetadataUbiquitousItemIsSharedKey: String

let NSMetadataUbiquitousSharedItemCurrentUserPermissionsKey: String

let NSMetadataUbiquitousSharedItemCurrentUserRoleKey: String

let NSMetadataUbiquitousSharedItemMostRecentEditorNameComponentsKey: String

let NSMetadataUbiquitousSharedItemOwnerNameComponentsKey: String

### iCloud Download Status Values

let NSMetadataUbiquitousItemDownloadingStatusCurrent: String

let NSMetadataUbiquitousItemDownloadingStatusDownloaded: String

let NSMetadataUbiquitousItemDownloadingStatusNotDownloaded: String

### iCloud Sharing Permissions Values

let NSMetadataUbiquitousSharedItemPermissionsReadOnly: String

let NSMetadataUbiquitousSharedItemPermissionsReadWrite: String

### iCloud Sharing Role Values

let NSMetadataUbiquitousSharedItemRoleOwner: String

let NSMetadataUbiquitousSharedItemRoleParticipant: String

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

### File Search

class NSMetadataQuery

A query that you perform against Spotlight metadata.

protocol NSMetadataQueryDelegate

An interface that enables the delegate of a metadata query to provide substitute results or attributes.

