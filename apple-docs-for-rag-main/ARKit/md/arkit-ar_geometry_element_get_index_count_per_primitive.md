

- ARKit
-  ar_geometry_element_get_index_count_per_primitive 

Function

# ar_geometry_element_get_index_count_per_primitive

Gets the number of indices for each primitive.

visionOS 1.0+

``` source
extern size_t ar_geometry_element_get_index_count_per_primitive(ar_geometry_element_t geometry_element);
```

## See Also

### Geometry

ar_geometry_primitive_type_t

The kinds of geometry primitives that a geometry element can contain.

ar_geometry_element_get_buffer

Gets a Metal buffer that contains index data that defines the geometry of an object.

ar_geometry_element_get_bytes_per_index

Gets the number of bytes that represent an index value.

ar_geometry_element_get_count

Gets the number of primitives in the Metal buffer for a geometry element.

ar_geometry_element_get_primitive_type

Gets the kind of primitive, lines or triangles, that a geometry element contains.

ar_geometry_source_get_buffer

Gets a Metal buffer that contains per-vector data for a geometry source.

ar_geometry_source_get_components_per_vector

Gets the number of scalar components in each vector in a geometry source.

ar_geometry_source_get_count

Gets the number of vectors in a geometry source.

ar_geometry_source_get_format

Gets the vertex format for data in a geometry source’s buffer.

ar_geometry_source_get_offset

Gets the offset, in bytes, from the beginning of a geometry source’s buffer.

ar_geometry_source_get_stride

Gets the number of bytes between one vector and another in a geometry source’s buffer.

ar_geometry_primitive_type_line

Two vertices that connect to form a line.

ar_geometry_primitive_type_triangle

Three vertices that connect to form a triangle.

ar_geometry_element_t

A container for vertex indices of lines or triangles.

ar_geometry_source_t

A container for geometrical vector data.

