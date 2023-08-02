# In Python, a hash map is typically implemented using the built-in dictionary data structure. 
A dictionary is an unordered collection of key-value pairs where each key must be unique. It allows for quick lookups, insertions, and deletions of elements based on their keys. Python's dictionary uses a hash table under the hood to achieve efficient data retrieval.

Here's how you can use a hash map (dictionary) in Python:

# Creating a hash map (dictionary):

# Method 1: Using curly braces and key-value pairs
my_dict = {'apple': 1, 'banana': 2, 'orange': 3}

# Method 2: Using the dict constructor and key-value pairs
my_dict = dict(apple=1, banana=2, orange=3)

# Method 3: Using a list of tuples containing key-value pairs
my_dict = dict([('apple', 1), ('banana', 2), ('orange', 3)])
Accessing elements in the hash map:

# Accessing value by key
print(my_dict['apple'])  # Output: 1

# Using the get() method to handle missing keys gracefully
print(my_dict.get('banana'))  # Output: 2
print(my_dict.get('grape', 'Not found'))  # Output: 'Not found' (default value for missing key)
Adding or updating elements in the hash map:

# Adding a new key-value pair
my_dict['grape'] = 4

# Updating the value of an existing key
my_dict['banana'] = 5
Deleting elements from the hash map:

# Deleting a key-value pair
del my_dict['orange']

# Using the pop() method to remove a key-value pair and return its value
removed_value = my_dict.pop('banana')
Checking if a key exists in the hash map:

if 'apple' in my_dict:
    print("Apple exists!")
Iterating through the hash map:

# Iterating through keys
for key in my_dict:
    print(key, my_dict[key])

# Iterating through key-value pairs
for key, value in my_dict.items():
    print(key, value)
It's important to note that dictionaries in Python maintain insertion order starting from Python 3.7 and are fully ordered in Python 3.8+. Before Python 3.7, dictionaries were unordered collections.
