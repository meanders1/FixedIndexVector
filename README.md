# FixedIndexVector

Simple vector with fixed indices. When an object is appended to the vector, an ID is received. The received ID is guaranteed to always point to the same element, unless the element itself is deleted.
IDs are reused when elements are deleted.

- Deletions: O(1)
- Additions: O(1) or O(n) if reallocation happens
- Access: O(1)
- 8 extra bytes per element
- Data is contiguous in memory
