[View code on GitHub](https://dune.com/docs/query/DuneSQL-reference/Functions-and-operators/array.md)

The app technical guide covers various array functions and operators used in SQL. It starts with the explanation of subscript operator `[]` used to access an element of an array, followed by the concatenation operator `||` used to concatenate arrays or elements of the same type.

The guide then dives into a comprehensive list of array functions, such as:

- `allmatch()`, `anymatch()`, `array_distinct()`, `array_except()`, `array_intersect()`, and `array_join()` for various array operations.
- `array_max()`, `array_min()`, `array_position()`, `array_remove()`, and `array_sort()` for sorting and finding elements in arrays.
- `array_union()`, `array_overlap()`, `cardinality()`, `concat()`, and `combinations()` for combining and manipulating arrays.
- `contains()`, `contains_sequence()`, `element_at()`, `filter()`, `flatten()`, and `ngrams()` for searching and filtering arrays.
- `none_match()`, `reduce()`, `repeat()`, `reverse()`, `sequence()`, `shuffle()`, `slice()`, `trim_array()`, `transform()`, `zip()`, and `zip_with()` for advanced array operations and transformations.

Each function is explained with its syntax, description, and examples to demonstrate its usage. This guide serves as a reference for users working with arrays in SQL, providing a detailed understanding of various array functions and operators.
## Questions: 
 1. **Question:** How does the `allmatch()` function handle empty arrays and NULL values in the input array?
   **Answer:** The `allmatch()` function returns `true` if the array is empty. If the predicate function returns `NULL` for one or more elements and `true` for all other elements, the `allmatch()` function returns `NULL`.

2. **Question:** What are the limitations of the `combinations()` function in terms of input array size and the value of `n`?
   **Answer:** The `combinations()` function has a limitation where `n` must not be greater than 5, and the total size of sub-groups generated must be smaller than 100,000.

3. **Question:** What is the difference between the `element_at()` function and the subscript operator `[]` when accessing elements in an array?
   **Answer:** The `element_at()` function returns `NULL` when accessing an index larger than the array length, whereas the subscript operator `[]` would fail in such a case. Additionally, if the index is negative, `element_at()` accesses elements from the last to the first.