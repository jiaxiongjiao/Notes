# Vertex Buffer

Any buffer can store vertex data. But for a buffer to be used a
vertex buffer, this buffer needs to be created with `VK_BUFFER_USAGE_VERTEX_BUFFER_BIT`.

Vertex buffer stores an array of structures which contains a bunch of information about a single vertex. Inside
vertex structure is a bunch of vertex attributes e.g. position, texture coordinate and color.

The stride of a vertex buffer is basically the size of the structure.
