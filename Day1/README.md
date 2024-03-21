## StringBuilder

A `StringBuilder` in Java is a class that provides an efficient way to create and manipulate strings. Strings in Java are immutable, meaning once created, their contents cannot be changed. This can lead to inefficiencies when performing operations that involve concatenation or modification of strings, as it requires creating new string objects each time.

`StringBuilder` addresses this issue by providing a mutable sequence of characters. It allows you to efficiently modify the contents of a string without creating new string objects each time. Here are some key points about `StringBuilder`:

- **Mutable**: Unlike strings, which are immutable, `StringBuilder` objects are mutable, meaning their content can be changed after they are created.
  
- **Efficient String Manipulation**: `StringBuilder` provides methods to append, insert, delete, and modify characters in the sequence, making it efficient for string manipulation tasks.
  
- **Performance**: Using `StringBuilder` for concatenating or modifying strings is generally more efficient than using string concatenation (`+`) or string manipulation methods like `substring`, especially when dealing with large strings or performing many concatenation operations.
  
- **Thread Safety**: Unlike `StringBuffer`, which is similar to `StringBuilder` but provides synchronization for use in multi-threaded environments, `StringBuilder` is not thread-safe. This makes it more efficient for single-threaded scenarios but requires external synchronization if used in a multi-threaded context.

### Constructor Summary

| Constructors                  | Constructor and Description                                                             |
|-------------------------------|-----------------------------------------------------------------------------------------|
| `StringBuilder()`            | Constructs a string builder with no characters in it and an initial capacity of 16 characters. |
| `StringBuilder(CharSequence seq)` | Constructs a string builder that contains the same characters as the specified `CharSequence`. |
| `StringBuilder(int capacity)`  | Constructs a string builder with no characters in it and an initial capacity specified by the capacity argument. |
| `StringBuilder(String str)`    | Constructs a string builder initialized to the contents of the specified string.           |

### Method Summary

#### All Methods

| Modifier and Type   | Method and Description                                                                   |
|---------------------|-------------------------------------------------------------------------------------------|
| `StringBuilder append(boolean b)`          | Appends the string representation of the boolean argument to the sequence.                       |
| `StringBuilder append(char c)`               | Appends the string representation of the char argument to this sequence.                            |
| `StringBuilder append(char[] str)`          | Appends the string representation of the char array argument to this sequence.                   |
| `StringBuilder append(char[] str, int offset, int len)` | Appends the string representation of a subarray of the char array argument to this sequence. |
| `StringBuilder append(CharSequence s)`    | Appends the specified character sequence to this Appendable.                                |
| `StringBuilder append(CharSequence s, int start, int end)` | Appends a subsequence of the specified CharSequence to this sequence.                       |
| `StringBuilder append(double d)`            | Appends the string representation of the double argument to this sequence.                         |
| `StringBuilder append(float f)`              | Appends the string representation of the float argument to this sequence.                              |
| `StringBuilder append(int i)`                    | Appends the string representation of the int argument to this sequence.                                         |
| `StringBuilder append(long lng)`            | Appends the string representation of the long argument to this sequence.                                          |
| `StringBuilder append(Object obj)`        | Appends the string representation of the Object argument.                                                                        |
| `StringBuilder append(String str)`             | Appends the specified string to this character sequence.                                                                                |
| `StringBuilder append(StringBuffer sb)` | Appends the specified StringBuffer to this sequence.                                                                                    |
| `StringBuilder appendCodePoint(int codePoint)` | Appends the string representation of the codePoint argument to this sequence.                                                |
| `int capacity()`                                          | Returns the current capacity.                                                                                                                             |
| `char charAt(int index)`                             | Returns the char value in this sequence at the specified index.                                                                                   |
| `int codePointAt(int index)`                        | Returns the character (Unicode code point) at the specified index.                                                                               |
| `int codePointBefore(int index)`                 | Returns the character (Unicode code point) before the specified index.                                                                        |
| `int codePointCount(int beginIndex, int endIndex)` | Returns the number of Unicode code points in the specified text range of this sequence.                                               |
| `StringBuilder delete(int start, int end)`        | Removes the characters in a substring of this sequence.                                                                                                      |
| `StringBuilder deleteCharAt(int index)`         | Removes the char at the specified position in this sequence.                                                                                           |
| `void ensureCapacity(int minimumCapacity)`   | Ensures that the capacity is at least equal to the specified minimum.                                                                          |
| `void getChars(int srcBegin, int srcEnd, char[] dst, int dstBegin)` | Characters are copied from this sequence into the destination character array dst.                                                  |
| `int indexOf(String str)`                              | Returns the index within this string of the first occurrence of the specified substring.                                                    |
| `int indexOf(String str, int fromIndex)`        | Returns the index within this string of the first occurrence of the specified substring, starting at the specified index.                  |
| `StringBuilder insert(int offset, boolean b)`    | Inserts the string representation of the boolean argument into this sequence.                                                                  |
| `StringBuilder insert(int offset, char c)`          | Inserts the string representation of the char argument into this sequence.                                                                            |
| `StringBuilder insert(int offset, char[] str)`   | Inserts the string representation of the char array argument into this sequence.                                                                   |
| `StringBuilder insert(int index, char[] str, int offset, int len)` | Inserts the string representation of a subarray of the str array argument into this sequence.                   |
| `StringBuilder insert(int dstOffset, CharSequence s)`        | Inserts the specified CharSequence into this sequence.                                                                                                              |
| `StringBuilder insert(int dstOffset, CharSequence s, int
