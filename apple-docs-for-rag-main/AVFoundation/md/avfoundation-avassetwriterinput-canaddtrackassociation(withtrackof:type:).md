

- AVFoundation
- AVAssetWriterInput
-  canAddTrackAssociation(withTrackOf:type:) 

Instance Method

# canAddTrackAssociation(withTrackOf:type:)

Determines whether it’s valid to associate another input’s track with this input’s track.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func canAddTrackAssociation(
    withTrackOf input: AVAssetWriterInput,
    type trackAssociationType: String
) -> Bool
```

## Parameters 

`input`  

An asset writer input that contains the track to associate.

`trackAssociationType`  

The type of track association to test.

## Return Value

true if the system can make the association between tracks; otherwise, false.

## Discussion

This method returns false if the association type requires tracks of a media type that doesn’t match the input’s type, or if the output file type doesn’t support track associations.

## See Also

### Configuring Track Associations

func addTrackAssociation(withTrackOf: AVAssetWriterInput, type: String)

Adds an association between input tracks.

