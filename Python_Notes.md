

### Invert a Dictionary

Inverting a dictionary means swapping its keys and values. The keys become values, and the values become keys. Here's a simple example in Python:

**Original dictionary**

original_dict = {'a': 1, 'b': 2, 'c': 3}

**Invert the dictionary**

inverted_dict = {v: k for k, v in original_dict.items()}

**Print the result**

print("Original Dictionary:", original_dict)
print("Inverted Dictionary:", inverted_dict)

### Combine Dictionary Values

If you have two dictionaries and you want to combine their values, you can achieve this by iterating through the dictionaries and combining the values for each key. Here's an example in Python:

**Two dictionaries**

dict1 = {'a': 1, 'b': 2, 'c': 3}
dict2 = {'a': 4, 'b': 5, 'd': 6}

**Combine dictionary values**
combined_dict = {}

**Iterate through dict1**
for key, value in dict1.items():
    combined_dict[key] = value + dict2.get(key, 0)

**Iterate through dict2 for keys not in dict1**
for key, value in dict2.items():
    if key not in dict1:
        combined_dict[key] = value

**Print the result**
print("Dictionary 1:", dict1)
print("Dictionary 2:", dict2)
print("Combined Dictionary:", combined_dict)



### Byte Size of String

In Python, the size of a string in terms of bytes depends on the encoding used to represent the characters in that string. The sys.getsizeof() function can be used to get the size of an object in bytes. However, keep in mind that this function returns the size of the object in memory, which includes not only the actual string data but also the overhead of the Python object itself.

Here's a simple example:

import sys

**Define a string**

my_string = "Hello, World!"

**Get the size of the string in bytes**

size_in_bytes = sys.getsizeof(my_string)

print(f"The size of the string is {size_in_bytes} bytes.")

The size of a string can vary based on the encoding and the number of characters. If you want to know the size of the string in terms of the number of bytes required to encode it in a specific encoding, you can use the encode() method:

**Define a string**

my_string = "Hello, World!"

**Encode the string using a specific encoding (e.g., UTF-8)**

encoded_string = my_string.encode('utf-8')

**Get the size of the encoded string in bytes**

size_in_bytes = len(encoded_string)

print(f"The size of the encoded string is {size_in_bytes} bytes.")

In this example, the encode('utf-8') method is used to encode the string in UTF-8, and then the length of the resulting byte sequence is used to determine the size in bytes. The actual size may also be influenced by factors like the presence of multi-byte characters, control characters, or other specific features of the encoding.

### Date Difference in Days

### Dictionary to List
