# Element-repetition-in-list-in-Python

# Apporach-1
# to perform element duplication  using list comprehension

# initializing list
test_list = [4, 5, 6, 3, 9]

# printing original list
print("The original list is : " + str(test_list))

# using list comprehension
# to perform element duplication
res = [i for i in test_list for x in (0, 1)]

# printing result
print("The list after element duplication " + str(res))

# Apporach-2

# to perform element duplication using reduce() + add
from operator import add

# initializing list
test_list = [4, 5, 6, 3, 9]

# printing original list
print("The original list is : " + str(test_list))

# using reduce() + add  to perform element duplication
res = list(reduce(add, [(i, i) for i in test_list]))

# printing result
print("The list after element duplication " + str(res))

# Apporach-3

test_list = [4, 5, 6, 3, 9]
# Printing the original list
print("The original list is:", test_list)
res = []
for i in test_list:
	res.extend([i, i])
print("The list after element duplication: " + str(res))


