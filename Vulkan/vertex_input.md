# Vertex Input

This stage import vertex data from [vertex buffer](vertex_buffer.md).

Vertex input use bindings to identify vertex buffers. Those bindings do not have to be continuous numbers.

`VkVertexInputBindingDescription` describes the vertex buffer binding number. It contains the binding number itself
and the stride of a vertex buffer, and input rate.

`VkVertexInputAttributeDescription` describes the location of this attribute in a shader. So this corresponds to
`(location = #)` in a shader. It uses `binding`, `format` and `offset` to know the location of the vertex attribute
you are describing here.

The maximum number of bindings is guranteed to be at least 16.

Each binding is an array of structures inside which contains all the information of each vertex. The stride of
of the binding is the distance between the start of each structure. The maximum value of a stride is gauranteed to
be 2048 byte.

---

# [[Questions]]
Isn't 16 a bit too few for a complete game?
