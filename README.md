# Python-Sets

## Objectives

1. Define Sets. 
2. How to create and use Sets with different methods
3. Why do we have to learn Sets?

## What is Sets? 

A Set is an unordered collection of items. It can have any number of items and they may be of different datatypes such as integer, float, tuple, string, and so on. However, a set cannot have a mutable element such as list, set, dictionary as its element. 

## Creating Sets
'''

test_set = {1, 3, 5}
test_set_mixed_datatypes = {0.5, "Hi", (2, 4, 6)}
empty_set = set()
'''
**Be careful with**
'''ruby
test_set_with_list = {1, [2, 3]}
#-> TyperError: unhashable type: 'list'
this_is_dictionary = {}
#-> Empty curly braces {} will make an empty dictionary, not a set
'''

## Methods for Sets

For Sets, there are few methods widely used: add, union, intersect, and difference.

1. Add method
people = {"Jay", "Idrish", "Archil"}
people.add("Daxit") 
-> This will add Daxit in people set.

output (print(people))
-> {'Archil', 'Idrish', 'Jay', 'Daxit'}

Frozen sets are almost same as normal sets, besides they are immutable.

'''python
normal_set = {"a", "b", "c"}
frozen_set = {"e", "f", "g"}
'''

Adding an element "d" to both normal and frozen set
'''python
normal_set.add("d")
frozen_set.add("d")

print(normal_set)
print(frozen_set)
'''
When you print normal_set only, result will be set(['a', 'c', 'b', 'd']) without any errors. However, when I also print frozen_set, I receive an attribute error, 'frozenset' object has no attribute 'add'.

<iframe width="560" height="315" src="https://www.youtube.com/embed/W0Q_AyfolRw" frameborder="0" allowfullscreen></iframe><p><a href="https://www.youtube.com/watch?v=WSgzIhgmJNE">How do normal and frozen sets work</a></p> 

2. remove Method
'''python
test_set = {1, 2, 3, 4}
test_set.remove(1)
-> {2, 3, 4}


3. union Method

set_A = {1, 2, 3}
set_B = {"Hi", "Hello"}
set_union = set_A.union(set_B) 
set_union_1 = set_B.union(set_A)
set_union_2 = set_A | set_B

#Three ways to compute union, and all same results
print(set_union)
print(set_union_1)
print(set_union_2)

-> {1, 2, 3, Hi, Hello}


4. intersect Method

set_A = {1, 2, 3}
set_B = {3, "Hi", "Hello"}
set_intersect = set_A.intersection(set_B)
set_intersect_1 = set_B.intersection(set_A)
set_intersect_2 = set_A & set_B

Three ways to compute inersect, and all same results
print(set_union)
print(set_union_1)
print(set_union_2)

-> {3}

5. difference(s) Method

set_A = {1, 2, 3}
set_B = {3, "Hi", "Hello"}
set_difference = set_A - set_B
set_intersect_1 = set_A.difference(set_B)
-> {1, 2}

set_difference = set_B - set_A
set_intersect_2 = set_B.difference(set_A)
-> {Hi, Hello}

## Importance of Data Structure 
As a coder, understading data structure is significantly important. Generally, algorithm is simpler when the data structure is very sophisticated. Simple algorithms are also less expensive to develop and less code to comprehend. Thus, this will let coders fix defects, make modifications, and add enhancements easier.

