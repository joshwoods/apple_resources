

- ARKit
- ARKit in visionOS C API
-  Objective-C compatibility 

API Collection

# Objective-C compatibility

## Topics

### Objective-C compatibility types

protocol OS_ar_anchor

The identity, location, and orientation of an object in world space.

protocol OS_ar_trackable_anchor

An anchor that can gain and lose its tracking state over the course of a session.

protocol OS_ar_authorization_result

An authorization result.

protocol OS_ar_authorization_results

A collection of authorization results.

protocol OS_ar_data_provider

A source of live data from ARKit.

protocol OS_ar_device_anchor

The position and orientation of Apple Vision Pro.

protocol OS_ar_error

An error reported by ARKit.

protocol OS_ar_data_providers

A source of live data from ARKit.

protocol OS_ar_geometry_element

A container for vertex indices of lines or triangles.

protocol OS_ar_geometry_source

A container for geometrical vector data.

protocol OS_ar_hand_anchor

A hand’s position in a person’s surroundings.

protocol OS_ar_hand_skeleton

protocol OS_ar_hand_tracking_provider

A source of live data about the position of a person’s hands and hand joints.

protocol OS_ar_hand_tracking_configuration

protocol OS_ar_image_tracking_configuration

protocol OS_ar_plane_detection_configuration

protocol OS_ar_plane_extent

The size of a plane.

protocol OS_ar_reference_images

A collection of reference images.

protocol OS_ar_scene_reconstruction_configuration

protocol OS_ar_session

The main entry point for receiving data from ARKit.

protocol OS_ar_world_tracking_configuration

protocol OS_ar_image_anchor

A 2D image’s position in a person’s surroundings.

protocol OS_ar_image_anchors

A collection of image anchors.

protocol OS_ar_image_tracking_provider

A source of live data about a 2D image’s position in a person’s surroundings.

protocol OS_ar_mesh_anchor

A source of live data about a 2D image’s position in a person’s surroundings.

protocol OS_ar_mesh_anchors

A collection of mech anchors.

protocol OS_ar_mesh_geometry

The shapes that make up a mesh anchor.

protocol OS_ar_plane_anchor

An anchor that represents horizontal and vertical planes.

protocol OS_ar_plane_anchors

A collection of plane anchors.

protocol OS_ar_plane_detection_provider

A source of live data about planes in a person’s surroundings.

protocol OS_ar_plane_geometry

The geometry of a plane anchor.

protocol OS_ar_reference_image

A 2D image the system uses as a reference to find the same image in a person’s surroundings.

protocol OS_ar_scene_reconstruction_provider

A source of live data about the shape of a person’s surroundings.

protocol OS_ar_skeleton_joint

protocol OS_ar_world_anchor

A fixed location in a person’s surroundings.

protocol OS_ar_world_anchors

A collection of world anchors.

protocol OS_ar_world_tracking_provider

A source of live data about the device pose and anchors in a person’s surroundings.

protocol OS_ar_barcode_anchor

protocol OS_ar_barcode_anchors

protocol OS_ar_barcode_detection_callbacks

protocol OS_ar_barcode_detection_configuration

protocol OS_ar_barcode_detection_provider

protocol OS_ar_camera_frame

protocol OS_ar_camera_frame_parameters

protocol OS_ar_camera_frame_provider

protocol OS_ar_camera_frame_sample

protocol OS_ar_camera_video_format

protocol OS_ar_camera_video_formats

protocol OS_ar_data

protocol OS_ar_environment_light_estimation_configuration

protocol OS_ar_environment_light_estimation_provider

protocol OS_ar_environment_probe_anchor

protocol OS_ar_environment_probe_anchors

protocol OS_ar_identifiers

protocol OS_ar_mesh_geometries

protocol OS_ar_object_anchor

protocol OS_ar_object_anchors

protocol OS_ar_object_axis_aligned_bounding_box

protocol OS_ar_object_tracking_configuration

protocol OS_ar_object_tracking_provider

protocol OS_ar_reference_object

protocol OS_ar_reference_objects

protocol OS_ar_room_anchor

protocol OS_ar_room_anchors

protocol OS_ar_room_tracking_configuration

protocol OS_ar_room_tracking_provider

var AR_OBJECT_USE_OBJC: Int32

AR_ASSUME_NONNULL_BEGIN

AR_ASSUME_NONNULL_END

AR_EXTERN

AR_MT_UNSAFE

AR_OBJECT_DECL

AR_OBJECT_DECL_SUBCLASS

AR_OBJECT_RETURNS_RETAINED

AR_REFINED_FOR_SWIFT

ar_release

ar_retain

## See Also

### Objective-C compatibility

ARKit Functions

ARKit Data Types

