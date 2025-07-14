

- AVFoundation
-  AVMetadataKey 

Structure

# AVMetadataKey

A structure that defines a metadata key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVMetadataKey
```

## Topics

### Common Metadata Keys

static let commonKeyAccessibilityDescription: AVMetadataKey

A key that represents the accessibility description for the media.

static let commonKeyAlbumName: AVMetadataKey

A key that represents the name of the album.

static let commonKeyArtist: AVMetadataKey

A key that represents the name of the artist.

static let commonKeyArtwork: AVMetadataKey

A key that represents an image relating to the album.

static let commonKeyAuthor: AVMetadataKey

A key that represents the name of the author.

static let commonKeyContributor: AVMetadataKey

A key that represents the name of the contributor.

static let commonKeyCopyrights: AVMetadataKey

A key that represents the copyright statement.

static let commonKeyCreationDate: AVMetadataKey

A key that represents the date of the original recording.

static let commonKeyCreator: AVMetadataKey

A key that represents the name of the creator.

static let commonKeyDescription: AVMetadataKey

A key that represents the description of the media.

static let commonKeyFormat: AVMetadataKey

A key that represents the file format of the media content.

static let commonKeyIdentifier: AVMetadataKey

A key that represents the ID for the media.

static let commonKeyLanguage: AVMetadataKey

A key that represents the language of the text or lyrics spoken or sung in the audio.

static let commonKeyLastModifiedDate: AVMetadataKey

A key that represents the last modification date of the media.

static let commonKeyLocation: AVMetadataKey

A key that represents the location information for the media.

static let commonKeyMake: AVMetadataKey

A key that represents the name of the camera maker.

static let commonKeyModel: AVMetadataKey

A key that represents the name of the camera model.

static let commonKeyPublisher: AVMetadataKey

A key that represents the name of the publisher.

static let commonKeyRelation: AVMetadataKey

A key that represents the relation information for the media.

static let commonKeySoftware: AVMetadataKey

A key that represents the name of the software used to create the media.

static let commonKeySource: AVMetadataKey

A key that represents the source information for the media.

static let commonKeySubject: AVMetadataKey

A key that represents the subject information for the media.

static let commonKeyTitle: AVMetadataKey

A key that represents the title of the media.

static let commonKeyType: AVMetadataKey

A key that represents the media type.

### iTunes Metadata Keys

static let iTunesMetadataKeyAccountKind: AVMetadataKey

A key that represents the kind of iTunes account.

static let iTunesMetadataKeyAcknowledgement: AVMetadataKey

A key that represents the acknowledgement information in iTunes.

static let iTunesMetadataKeyAlbum: AVMetadataKey

A key that represents the name of the album in iTunes.

static let iTunesMetadataKeyAlbumArtist: AVMetadataKey

A key that represents the artist for the album.

static let iTunesMetadataKeyAppleID: AVMetadataKey

A key that represents an Apple ID.

static let iTunesMetadataKeyArranger: AVMetadataKey

A key that represents the name of the arranger.

static let iTunesMetadataKeyArtDirector: AVMetadataKey

A key that represents the name of the art director.

static let iTunesMetadataKeyArtist: AVMetadataKey

A key that represents the name of the artist.

static let iTunesMetadataKeyArtistID: AVMetadataKey

A key that represents the ID for an artist.

static let iTunesMetadataKeyAuthor: AVMetadataKey

A key that represents the name of the author.

static let iTunesMetadataKeyBeatsPerMin: AVMetadataKey

A key that represents the beats per minute of a track in iTunes.

static let iTunesMetadataKeyComposer: AVMetadataKey

A key that represents the name of the composer.

static let iTunesMetadataKeyConductor: AVMetadataKey

A key that represents the name of the conductor.

static let iTunesMetadataKeyContentRating: AVMetadataKey

A key that represents the content rating in iTunes.

static let iTunesMetadataKeyCopyright: AVMetadataKey

A key that represents the copyright statement in iTunes.

static let iTunesMetadataKeyCoverArt: AVMetadataKey

A key that represents an album cover image.

static let iTunesMetadataKeyCredits: AVMetadataKey

A key that represents the credits for the source content.

static let iTunesMetadataKeyDescription: AVMetadataKey

A key that represents the description information in iTunes.

static let iTunesMetadataKeyDirector: AVMetadataKey

A key that represents the name of the director.

static let iTunesMetadataKeyDiscCompilation: AVMetadataKey

A key that represents whether an album is a compilation of tracks in iTunes.

static let iTunesMetadataKeyDiscNumber: AVMetadataKey

A key that represents the disc number of a multi-CD album in iTunes.

static let iTunesMetadataKeyEncodedBy: AVMetadataKey

A key that represents the person or organization that encoded the media.

static let iTunesMetadataKeyEncodingTool: AVMetadataKey

A key that represents the software or hardware and settings used for encoding.

static let iTunesMetadataKeyEQ: AVMetadataKey

A key that represents the equalizer preset option in iTunes.

static let iTunesMetadataKeyExecProducer: AVMetadataKey

A key that represents the name of the executive producer.

static let iTunesMetadataKeyGenreID: AVMetadataKey

A key that represents the genre ID.

static let iTunesMetadataKeyGrouping: AVMetadataKey

A key that represents additional grouping information for an album.

static let iTunesMetadataKeyLinerNotes: AVMetadataKey

A key that represents the digital booklet for an album.

static let iTunesMetadataKeyLyrics: AVMetadataKey

A key that represents the lyrics in the recording.

static let iTunesMetadataKeyOnlineExtras: AVMetadataKey

A key that represents the extra materials for an album.

static let iTunesMetadataKeyOriginalArtist: AVMetadataKey

A key that represents the name of the original artist.

static let iTunesMetadataKeyPerformer: AVMetadataKey

A key that represents the name of the performer.

static let iTunesMetadataKeyPhonogramRights: AVMetadataKey

A key that represents the phonogram rights statement.

static let iTunesMetadataKeyPlaylistID: AVMetadataKey

A key that represents the playlist ID.

static let iTunesMetadataKeyPredefinedGenre: AVMetadataKey

A key that represents the predefined genre.

static let iTunesMetadataKeyProducer: AVMetadataKey

A key that represents the name of the producer.

static let iTunesMetadataKeyPublisher: AVMetadataKey

A key that represents the name of the publisher.

static let iTunesMetadataKeyRecordCompany: AVMetadataKey

A key that represents the name of the record company.

static let iTunesMetadataKeyReleaseDate: AVMetadataKey

A key that represents the release date for the original recording.

static let iTunesMetadataKeySoloist: AVMetadataKey

A key that represents the name of the soloist.

static let iTunesMetadataKeySongID: AVMetadataKey

A key that represents the song ID.

static let iTunesMetadataKeySongName: AVMetadataKey

A key that represents the name of the song in iTunes.

static let iTunesMetadataKeySoundEngineer: AVMetadataKey

A key that represents the name of the sound engineer.

static let iTunesMetadataKeyThanks: AVMetadataKey

A key that represents the thanks statement in iTunes.

static let iTunesMetadataKeyTrackNumber: AVMetadataKey

A key that represents the order number in iTunes.

static let iTunesMetadataKeyTrackSubTitle: AVMetadataKey

A key that represents the information relating to the contents title.

static let iTunesMetadataKeyUserComment: AVMetadataKey

A key that represents a user comment regarding the content.

static let iTunesMetadataKeyUserGenre: AVMetadataKey

A key that represents the genre set by a user in iTunes.

### QuickTime Metadata Keys

static let quickTimeMetadataKeyAccessibilityDescription: AVMetadataKey

A key that represents the accessibility description for the movie file content.

static let quickTimeMetadataKeyAlbum: AVMetadataKey

A key that represents the name of the album or collection in QuickTime.

static let quickTimeMetadataKeyArranger: AVMetadataKey

A key that represents the name of the arranger of the movie file content.

static let quickTimeMetadataKeyArtist: AVMetadataKey

A key that represents the name of the artist of the movie file content.

static let quickTimeMetadataKeyArtwork: AVMetadataKey

A key that represents an image relating to the movie file content.

static let quickTimeMetadataKeyAuthor: AVMetadataKey

A key that represents the name of the author of the movie file content.

static let quickTimeMetadataKeyCameraFrameReadoutTime: AVMetadataKey

A key that represents the camera frame readout time in QuickTime.

static let quickTimeMetadataKeyCameraIdentifier: AVMetadataKey

A key that represents the camera identifier in QuickTime.

static let quickTimeMetadataKeyCollectionUser: AVMetadataKey

A key that represents a name that indicates a user-defined collection.

static let quickTimeMetadataKeyComment: AVMetadataKey

A key that represents a comment regarding the movie file content.

static let quickTimeMetadataKeyComposer: AVMetadataKey

A key that represents the name of the composer of the movie file content.

static let quickTimeMetadataKeyContentIdentifier: AVMetadataKey

A key that represents the content identifier in QuickTime.

static let quickTimeMetadataKeyCopyright: AVMetadataKey

A key that represents the copyright statement for the movie file content.

static let quickTimeMetadataKeyCreationDate: AVMetadataKey

A key that represents the creation date of the movie file content.

static let quickTimeMetadataKeyCredits: AVMetadataKey

A key that represents the credits of the movie source content.

static let quickTimeMetadataKeyDescription: AVMetadataKey

A key that represents the description of the movie file content.

static let quickTimeMetadataKeyDirectionFacing: AVMetadataKey

A key that represents the direction the camera is facing during the shot.

static let quickTimeMetadataKeyDirectionMotion: AVMetadataKey

A key that represents the direction the camera is moving during the shot.

static let quickTimeMetadataKeyDirector: AVMetadataKey

A key that represents the name of the director of the movie file content.

static let quickTimeMetadataKeyDisplayName: AVMetadataKey

A key that represents the display name of the movie file content.

static let quickTimeMetadataKeyEncodedBy: AVMetadataKey

A key that represents the name of the person or organization responsible for encoding the movie file content.

static let quickTimeMetadataKeyFullFrameRatePlaybackIntent: AVMetadataKey

An key that represents whether this movie should play at full frame rate.

static let quickTimeMetadataKeyGenre: AVMetadataKey

A key that represents the genre or genres to which the movie content conforms.

static let quickTimeMetadataKeyInformation: AVMetadataKey

A key that represents general information about the movie file content.

static let quickTimeMetadataKeyIsMontage: AVMetadataKey

A key that represents that the movie is a montage of other media.

static let quickTimeMetadataKeyiXML: AVMetadataKey

A key that represents iXML information for the movie file content.

static let quickTimeMetadataKeyKeywords: AVMetadataKey

A key that represents the keywords for the movie file content.

static let quickTimeMetadataKeyLocationBody: AVMetadataKey

A key that represents the astronomical body for compatibility with the 3GPP format.

static let quickTimeMetadataKeyLocationDate: AVMetadataKey

A key that represents a date and time using the extended format defined in ISO 8601:2004.

static let quickTimeMetadataKeyLocationISO6709: AVMetadataKey

A key that represents the geographic point location by coordinates as defined in ISO 6709:2008.

static let quickTimeMetadataKeyLocationName: AVMetadataKey

A key that represents the name of the location.

static let quickTimeMetadataKeyLocationNote: AVMetadataKey

A key that represents a descriptive comment about the location.

static let quickTimeMetadataKeyLocationRole: AVMetadataKey

A key that represents the single byte describing the movie location.

static let quickTimeMetadataKeyMake: AVMetadataKey

A key that represents the name of the camera maker.

static let quickTimeMetadataKeyModel: AVMetadataKey

A key that represents the name of the camera model.

static let quickTimeMetadataKeyOriginalArtist: AVMetadataKey

A key that represents the name of the original artist of the movie file content.

static let quickTimeMetadataKeyPerformer: AVMetadataKey

A key that represents the name of the performer in the movie file content.

static let quickTimeMetadataKeyPhonogramRights: AVMetadataKey

A key that represents the phonogram rights statement.

static let quickTimeMetadataKeyProducer: AVMetadataKey

A key that represents the name of the producer of the movie file content.

static let quickTimeMetadataKeyPublisher: AVMetadataKey

A key that represents the name of the publisher of the movie file content.

static let quickTimeMetadataKeyRatingUser: AVMetadataKey

A key that represents the rating or relative value of the movie.

static let quickTimeMetadataKeySoftware: AVMetadataKey

A key that represents the name of software used to create the movie file content.

static let quickTimeMetadataKeyTitle: AVMetadataKey

A key that represents the title of the movie file content.

static let quickTimeMetadataKeyYear: AVMetadataKey

A key that represents the recording year of the movie file content.

### QuickTime User Metadata Keys

static let quickTimeUserDataKeyAccessibilityDescription: AVMetadataKey

A key that represents the accessibility description for the movie file content.

static let quickTimeUserDataKeyAlbum: AVMetadataKey

A key that represents the name of the album or collection in QuickTime.

static let quickTimeUserDataKeyArranger: AVMetadataKey

A key that represents the name of the arranger of the movie file content.

static let quickTimeUserDataKeyArtist: AVMetadataKey

A key that represents the name of the artist of the movie file content.

static let quickTimeUserDataKeyAuthor: AVMetadataKey

A key that represents the name of the author of the movie file content.

static let quickTimeUserDataKeyChapter: AVMetadataKey

A key that represents the name of the chapter.

static let quickTimeUserDataKeyComment: AVMetadataKey

A key that represents a comment regarding the movie file content.

static let quickTimeUserDataKeyComposer: AVMetadataKey

A key that represents the name of the composer of the movie file content.

static let quickTimeUserDataKeyCopyright: AVMetadataKey

A key that represents the copyright statement in QuickTime.

static let quickTimeUserDataKeyCreationDate: AVMetadataKey

A key that represents the creation date of the movie file content.

static let quickTimeUserDataKeyCredits: AVMetadataKey

A key that represents the credits of movie source content.

static let quickTimeUserDataKeyDescription: AVMetadataKey

A key that represents the description of the movie file content.

static let quickTimeUserDataKeyDirector: AVMetadataKey

A key that represents the name of the director of the movie file content.

static let quickTimeUserDataKeyDisclaimer: AVMetadataKey

A key that represents the disclaimer regarding the movie file content.

static let quickTimeUserDataKeyEncodedBy: AVMetadataKey

A key that represents the name of the person or organization responsible for encoding the movie file content.

static let quickTimeUserDataKeyFullName: AVMetadataKey

A key that represents the full name of the movie file content.

static let quickTimeUserDataKeyGenre: AVMetadataKey

A key that represents the genre or genres to which the movie content conforms.

static let quickTimeUserDataKeyHostComputer: AVMetadataKey

A key that represents the name of the host computer.

static let quickTimeUserDataKeyInformation: AVMetadataKey

A key that represents general information about the movie file content.

static let quickTimeUserDataKeyKeywords: AVMetadataKey

A key that represents the keywords for the movie file content.

static let quickTimeUserDataKeyLocationISO6709: AVMetadataKey

A key that represents the geographic point location by coordinates as defined in ISO 6709:2008.

static let quickTimeUserDataKeyMake: AVMetadataKey

A key that represents the name of the camera maker.

static let quickTimeUserDataKeyModel: AVMetadataKey

A key that represents the name of the camera model.

static let quickTimeUserDataKeyOriginalArtist: AVMetadataKey

A key that represents the name of the original artist of the movie file content.

static let quickTimeUserDataKeyOriginalFormat: AVMetadataKey

A key that represents the original format of the movie file content.

static let quickTimeUserDataKeyOriginalSource: AVMetadataKey

A key that represents the original source of the movie file content.

static let quickTimeUserDataKeyPerformers: AVMetadataKey

A key that represents the name of the performers in the movie file content.

static let quickTimeUserDataKeyPhonogramRights: AVMetadataKey

A key that represents the phonogram rights statement.

static let quickTimeUserDataKeyProducer: AVMetadataKey

A key that represents the name of the producer of the movie file content.

static let quickTimeUserDataKeyProduct: AVMetadataKey

A key that represents the name of the product.

static let quickTimeUserDataKeyPublisher: AVMetadataKey

A key that represents the name of the publisher of the movie file content.

static let quickTimeUserDataKeySoftware: AVMetadataKey

A key that represents the name of software used to create the movie file content.

static let quickTimeUserDataKeySpecialPlaybackRequirements: AVMetadataKey

A key that represents the special hardware and software requirements for playback.

static let quickTimeUserDataKeyTaggedCharacteristic: AVMetadataKey

A key that represents the tagged characteristic.

static let quickTimeUserDataKeyTrack: AVMetadataKey

A key that represents a track in the movie file content.

static let quickTimeUserDataKeyTrackName: AVMetadataKey

A key that represents the name of a track in the movie file content.

static let quickTimeUserDataKeyURLLink: AVMetadataKey

A key that represents the webpage for the movie file content.

static let quickTimeUserDataKeyWarning: AVMetadataKey

A key that represents the warning text for the movie file content.

static let quickTimeUserDataKeyWriter: AVMetadataKey

A key that represents the name of the writer of the movie file content.

### ID3 Metadata Keys

static let id3MetadataKeyAlbumSortOrder: AVMetadataKey

A key that represents how to sort the album.

static let id3MetadataKeyAlbumTitle: AVMetadataKey

A key that represents the title of the recording.

static let id3MetadataKeyAttachedPicture: AVMetadataKey

A key that represents an image relating to the audio file.

static let id3MetadataKeyAudioEncryption: AVMetadataKey

A key that represents the encryption details of the audio stream.

static let id3MetadataKeyAudioSeekPointIndex: AVMetadataKey

A key that represents the list of seek points within the audio file.

static let id3MetadataKeyBand: AVMetadataKey

A key that represents additional information about the performers in the recording.

static let id3MetadataKeyBeatsPerMinute: AVMetadataKey

A key that represents the beats per minute of the audio.

static let id3MetadataKeyComments: AVMetadataKey

A key that represents additional text information for the media.

static let id3MetadataKeyCommercial: AVMetadataKey

A key that represents the commercial details for the media.

static let id3MetadataKeyCommercialInformation: AVMetadataKey

A key that represents the webpage containing purchasing information.

static let id3MetadataKeyComposer: AVMetadataKey

A key that represents the name of the composer.

static let id3MetadataKeyConductor: AVMetadataKey

A key that represents the name of the conductor.

static let id3MetadataKeyContentGroupDescription: AVMetadataKey

A key that indicates the sound belongs to a larger category of sounds or music.

static let id3MetadataKeyContentType: AVMetadataKey

A key that represents the media content type.

static let id3MetadataKeyCopyright: AVMetadataKey

A key that represents the copyright statement.

static let id3MetadataKeyCopyrightInformation: AVMetadataKey

A key that represents the webpage describing the terms of use and ownership.

static let id3MetadataKeyDate: AVMetadataKey

A key that represents the date for the recording.

static let id3MetadataKeyEncodedBy: AVMetadataKey

A key that represents the person or organization responsible for encoding the media.

static let id3MetadataKeyEncodedWith: AVMetadataKey

A key that represents the software or hardware and settings used for encoding.

static let id3MetadataKeyEncodingTime: AVMetadataKey

A key that represents the encoding time of the audio.

static let id3MetadataKeyEncryption: AVMetadataKey

A key that represents the encryption method used.

static let id3MetadataKeyEqualization: AVMetadataKey

A key that represents the equalization curve within the audio file.

static let id3MetadataKeyEqualization2: AVMetadataKey

A key that represents the equalization curve within the audio file.

static let id3MetadataKeyEventTimingCodes: AVMetadataKey

A key that represents the timing codes used for synchronization with key events in a song or sound.

static let id3MetadataKeyFileOwner: AVMetadataKey

A key that represents the name of the owner or licensee of the file and it’s contents.

static let id3MetadataKeyFileType: AVMetadataKey

A key that represents the file type of the audio.

static let id3MetadataKeyGeneralEncapsulatedObject: AVMetadataKey

A key that represents the details of a file.

static let id3MetadataKeyGroupIdentifier: AVMetadataKey

A key that represents the grouping of distinct frames.

static let id3MetadataKeyInitialKey: AVMetadataKey

A key that represents the musical key in which the sound starts.

static let id3MetadataKeyInternationalStandardRecordingCode: AVMetadataKey

A key that represents the international standard recording code.

static let id3MetadataKeyInternetRadioStationName: AVMetadataKey

A key that represents the name of the internet radio station streaming the audio.

static let id3MetadataKeyInternetRadioStationOwner: AVMetadataKey

A key that represents the name of the owner of the internet radio station streaming the audio.

static let id3MetadataKeyInvolvedPeopleList_v23: AVMetadataKey

A key that represents the list of names of contributors to the media.

static let id3MetadataKeyInvolvedPeopleList_v24: AVMetadataKey

A key that represents the list of names of contributors to the media.

static let id3MetadataKeyLanguage: AVMetadataKey

A key that represents the language of the text or lyrics spoken or sung in the audio.

static let id3MetadataKeyLeadPerformer: AVMetadataKey

A key that represents the main artist of the recording.

static let id3MetadataKeyLength: AVMetadataKey

A key that represents the length of the audio file in milliseconds.

static let id3MetadataKeyLink: AVMetadataKey

A key that represents the link information from an ID3 tag that might reside in another audio file or alone in a binary file.

static let id3MetadataKeyLyricist: AVMetadataKey

A key that represents the writer(s) of the text or lyrics in the recording.

static let id3MetadataKeyMediaType: AVMetadataKey

A key that represents which media the sound originated from.

static let id3MetadataKeyModifiedBy: AVMetadataKey

A key that represents the people behind a remix and similar interpretations of another existing piece.

static let id3MetadataKeyMood: AVMetadataKey

A key that represents the mood of the audio.

static let id3MetadataKeyMPEGLocationLookupTable: AVMetadataKey

A key that represents the lookup table used to increase performance and accuracy of jumps within an MPEG audio file.

static let id3MetadataKeyMusicCDIdentifier: AVMetadataKey

A key that represents the ID used to identify the CD in databases such as the Compact Disc Database.

static let id3MetadataKeyMusicianCreditsList: AVMetadataKey

A key that represents the mapping between an instrument and the musician that played it.

static let id3MetadataKeyOfficialArtistWebpage: AVMetadataKey

A key that represents the artist’s official webpage.

static let id3MetadataKeyOfficialAudioFileWebpage: AVMetadataKey

A key that represents the official webpage for the audio file.

static let id3MetadataKeyOfficialAudioSourceWebpage: AVMetadataKey

A key that represents the official webpage for the source of the audio file.

static let id3MetadataKeyOfficialInternetRadioStationHomepage: AVMetadataKey

A key that represents the official homepage of the internet radio station.

static let id3MetadataKeyOfficialPublisherWebpage: AVMetadataKey

A key that represents the official webpage for the publisher.

static let id3MetadataKeyOriginalAlbumTitle: AVMetadataKey

A key that represents the title of the original recording or source of sound.

static let id3MetadataKeyOriginalArtist: AVMetadataKey

A key that represents the performer(s) of the original recording.

static let id3MetadataKeyOriginalFilename: AVMetadataKey

A key that represents the original filename for the recording.

static let id3MetadataKeyOriginalLyricist: AVMetadataKey

A key that represents the text writer(s) of the original recording.

static let id3MetadataKeyOriginalReleaseTime: AVMetadataKey

A key that represents the release time for the original recording.

static let id3MetadataKeyOriginalReleaseYear: AVMetadataKey

A key that represents the release year for the original recording.

static let id3MetadataKeyOwnership: AVMetadataKey

A key that represents the transaction details indicating proof of ownership if signed.

static let id3MetadataKeyPartOfASet: AVMetadataKey

A key that represents the part of a set the audio came from.

static let id3MetadataKeyPayment: AVMetadataKey

A key that represents the webpage that handles the process of paying for the audio file.

static let id3MetadataKeyPerformerSortOrder: AVMetadataKey

A key that represents the performer sort order.

static let id3MetadataKeyPlayCounter: AVMetadataKey

A key that represents the play count of the audio file.

static let id3MetadataKeyPlaylistDelay: AVMetadataKey

A key that represents the number of milliseconds of silence between every song in a playlist.

static let id3MetadataKeyPopularimeter: AVMetadataKey

A key that represents the rating for the audio file.

static let id3MetadataKeyPositionSynchronization: AVMetadataKey

A key that represents the time offset of the first frame in the stream.

static let id3MetadataKeyPrivate: AVMetadataKey

A key that represents the information from a software producer that its program uses.

static let id3MetadataKeyProducedNotice: AVMetadataKey

A key that represents the produced notice.

static let id3MetadataKeyPublisher: AVMetadataKey

A key that represents the name of the label or publisher.

static let id3MetadataKeyRecommendedBufferSize: AVMetadataKey

A key that represents the buffer size the server recommends.

static let id3MetadataKeyRecordingDates: AVMetadataKey

A key that represents additional recording dates that complement year, date, and time keys.

static let id3MetadataKeyRecordingTime: AVMetadataKey

A key that represents the recording time.

static let id3MetadataKeyRelativeVolumeAdjustment: AVMetadataKey

A key that represents the increase or decrease of volume on each channel while the file plays.

static let id3MetadataKeyRelativeVolumeAdjustment2: AVMetadataKey

A key that represents the increase or decrease of volume on each channel while the file plays.

static let id3MetadataKeyReleaseTime: AVMetadataKey

A key that represents the time of the first release.

static let id3MetadataKeyReverb: AVMetadataKey

A key that represents the adjustments to echoes of different kinds.

static let id3MetadataKeySeek: AVMetadataKey

A key that represents the location of other tags in a file or stream.

static let id3MetadataKeySetSubtitle: AVMetadataKey

A key that represents the set subtitle the track belongs to.

static let id3MetadataKeySignature: AVMetadataKey

A key that represents the group of frames to sign.

static let id3MetadataKeySize: AVMetadataKey

A key that represents the size of the audio file in bytes.

static let id3MetadataKeySubTitle: AVMetadataKey

A key that represents the information relating to the contents title.

static let id3MetadataKeySynchronizedLyric: AVMetadataKey

A key that represents the words in the audio file as text in sync with the audio.

static let id3MetadataKeySynchronizedTempoCodes: AVMetadataKey

A key that represents the tempo codes used for a more accurate description of the tempo of a musical piece.

static let id3MetadataKeyTaggingTime: AVMetadataKey

A key that represents the time of tagging.

static let id3MetadataKeyTermsOfUse: AVMetadataKey

A key that represents the brief description of the terms of use and ownership of the file.

static let id3MetadataKeyTime: AVMetadataKey

A key that represents the time for the recording.

static let id3MetadataKeyTitleDescription: AVMetadataKey

A key that represents the name of the piece.

static let id3MetadataKeyTitleSortOrder: AVMetadataKey

A key that represents the title sort order.

static let id3MetadataKeyTrackNumber: AVMetadataKey

A key that represents the order number of the audio file.

static let id3MetadataKeyUniqueFileIdentifier: AVMetadataKey

A key that represents the identifier used to indicate the audio file in a database.

static let id3MetadataKeyUnsynchronizedLyric: AVMetadataKey

A key that represents the lyrics of the song or a text transcription of other vocal activities.

static let id3MetadataKeyUserText: AVMetadataKey

A key that represents the user text information frame.

static let id3MetadataKeyUserURL: AVMetadataKey

A key that represents the user webpage frame.

static let id3MetadataKeyYear: AVMetadataKey

A key that represents the year of the recording.

static let id3MetadataKeyCommerical: AVMetadataKey

A key that represents the commerical frame.

Deprecated

### 3GP User Metadata Keys

static let metadata3GPUserDataKeyAlbumAndTrack: AVMetadataKey

A key that represents the text for the album and track titles.

static let metadata3GPUserDataKeyAuthor: AVMetadataKey

A key that represents the author of the media.

static let metadata3GPUserDataKeyCollection: AVMetadataKey

A key that represents the collection name for the media.

static let metadata3GPUserDataKeyCopyright: AVMetadataKey

A key that represents the copyright statement.

static let metadata3GPUserDataKeyDescription: AVMetadataKey

A key that represents the description for the media.

static let metadata3GPUserDataKeyGenre: AVMetadataKey

A key that represents the genre of the media.

static let metadata3GPUserDataKeyKeywordList: AVMetadataKey

A key that represents the list of keywords for the media.

static let metadata3GPUserDataKeyLocation: AVMetadataKey

A key that represents the location information for the media.

static let metadata3GPUserDataKeyMediaClassification: AVMetadataKey

A key that represents the classification of the media content.

static let metadata3GPUserDataKeyMediaRating: AVMetadataKey

A key that represents the rating of the media content.

static let metadata3GPUserDataKeyPerformer: AVMetadataKey

A key that represents information about the performer.

static let metadata3GPUserDataKeyRecordingYear: AVMetadataKey

A key that represents the recording year for the media.

static let metadata3GPUserDataKeyThumbnail: AVMetadataKey

A key that represents the media thumbnail.

static let metadata3GPUserDataKeyTitle: AVMetadataKey

A key that represents the title for the media.

static let metadata3GPUserDataKeyUserRating: AVMetadataKey

A key that represents the user rating.

### ISO User Metadata Keys

static let isoUserDataKeyAccessibilityDescription: AVMetadataKey

A key that represents the accessibility description for the media content.

static let isoUserDataKeyCopyright: AVMetadataKey

A key that represents the copyright statement.

static let isoUserDataKeyDate: AVMetadataKey

A key that represents the date for the media content.

static let isoUserDataKeyTaggedCharacteristic: AVMetadataKey

A key that represents the tagged media characteristic used for identifying accessibility features.

### ICY Metadata Keys

static let icyMetadataKeyStreamTitle: AVMetadataKey

A key that represents the title of a stream.

static let icyMetadataKeyStreamURL: AVMetadataKey

A key that represents the web address of a stream.

### Initializers

init(String)

Creates a metadata key.

init(rawValue: String)

Creates a metadata key with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Metadata

Retrieving media metadata

Load descriptive metadata for media assets and their tracks.

class AVMetadataItem

A metadata item for an audiovisual asset or one of its tracks.

class AVMutableMetadataItem

A mutable metadata item for an audiovisual asset or for one of its tracks.

struct AVMetadataIdentifier

A structure that defines identifiers for metadata formats.

struct AVMetadataKeySpace

A structure that defines a metadata key space.

struct AVMetadataExtraAttributeKey

A structure that defines keys for extra metadata attributes.

struct AVMetadataFormat

A structure that defines metadata formats.

class AVMetadataItemFilter

An object that filters selected information from a metadata item.

