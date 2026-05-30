# Assignment-no.8


# Sample dictionary
data = {'apple': 10, 'orange': 5, 'banana': 25, 'mango': 15}

# Sorting ascending
sorted_asc = dict(sorted(data.items(), key=lambda item: item[1]))

# Sorting descending
sorted_desc = dict(sorted(data.items(), key=lambda item: item[1], reverse=True))

print("Original:", data)
print("Ascending:", sorted_asc)
print("Descending:", sorted_desc


output 

Original: {'apple': 10, 'orange': 5, 'banana': 25, 'mango': 15}
Ascending: {'orange': 5, 'apple': 10, 'mango': 15, 'banana': 25}
Descending: {'banana': 25, 'mango': 15, 'apple': 10, 'orange': 5}


my_dict = {'a': 100, 'b': 200, 'c': 300}

def check_key(dictionary, key):
    if key in dictionary:
        print(f"Key '{key}' exists in the dictionary.")
    else:
        print(f"Key '{key}' does not exist.")

check_key(my_dict, 'b')
check_key(my_dict, 'z')


output 


Key 'b' exists in the dictionary.
Key 'z' does not exist.



dict1 = {'a': 1, 'b': 2}
dict2 = {'b': 99, 'c': 4}  # 'b' will be updated with dict2's value

# Using the | operator (Python 3.9+)
merged_dict = dict1 | dict2

print("Merged dictionary:", merged_dict)

output 

Merged dictionary: {'a': 1, 'b': 99, 'c': 4}






original_tuple = (1, 2, 3)
new_item = 4

# Concatenating tuples (notice the comma after new_item)
updated_tuple = original_tuple + (new_item,)

print("Original tuple:", original_tuple)
print("Updated tuple:", updated_tuple)


output 

Original tuple: (1, 2, 3)
Updated tuple: (1, 2, 3, 4)







mixed_tuple = ("Python", 42, 3.14, True, [1, 2])

print("Mixed Tuple:", mixed_tuple)
for item in mixed_tuple:
    print(f"Item: {item} -> Type: {type(item).__name__}")

output 


Mixed Tuple: ('Python', 42, 3.14, True, [1, 2])
Item: Python -> Type: str
Item: 42 -> Type: int
Item: 3.14 -> Type: float
Item: True -> Type: bool
Item: [1, 2] -> Type: list





numbers = [10, 20, 30, 40, 50]

total_sum = sum(numbers)

print("List:", numbers)
print("Sum of items:", total_sum

output 

List: [10, 20, 30, 40, 50]
Sum of items: 150






numbers = [45, 12, 89, 5, 67]

largest = max(numbers)

print("List:", numbers)
print("Largest number:", largest)



output 


List: [45, 12, 89, 5, 67]
Largest number: 89





my_set = {1, 2, 3}

# Add a single member
my_set.add(4)

# Add multiple members
my_set.update([5, 6, 2]) # 2 is a duplicate, so it won't be repeated

print("Updated set:", my_set)


output 

Updated set: {1, 2, 3, 4, 5, 6}




import array as arr

# Creating an integer array
my_array = arr.array('i', [1, 2, 3, 4, 5])
print("Original array:", list(my_array))

# Reversing the array in place
my_array.reverse()

print("Reversed array:", list(my_array))

output 

Original array: [1, 2, 3, 4, 5]
Reversed array: [5, 4, 3, 2, 1]



import array as arr

# Create an array of 5 integers ('i' represents signed integer)
numbers = arr.array('i', [10, 20, 30, 40, 50])

# Displaying all items
print("Displaying all array items:")
for item in numbers:
    print(item, end=" ")
print("\n" + "-"*30)

# Accessing elements through indexes
print("Accessing individual elements:")
print("Element at index 0:", numbers[0])
print("Element at index 2:", numbers[2])
print("Element at index 4:", numbers[4])


output 

Displaying all array items:
10 20 30 40 50 
------------------------------
Accessing individual elements:
Element at index 0: 10
Element at index 2: 30
Element at index 4: 50