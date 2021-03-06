# List Methods 13

### !challenge

* type: code-snippet
* language: python3.6
* id: 54143016-2767-47af-9931-408799951ba0
* title: get_largest_element

### !question

Write a function called "get_largest_element".

Given a list, "get_largest_element" returns the largest number in the given list.

Notes:
* It should return 0 if the list is empty.

```
output = get_largest_element([5, 2, 8, 3])
print(output) # --> 8
```

### !end-question

### !placeholder

```python
# your code here



```

### !end-placeholder

### !tests

```python
import main
import unittest

class TestScript(unittest.TestCase):
    def test_0(self):
        # it should return a number
        self.assertIsInstance(main.get_largest_element([3, 5, 3, 1]), (float, int),
        msg = 'should return a number')


    def test_1(self):
        # it should return the largest element in a list
        self.assertEqual(main.get_largest_element([3, 5, 3, 1]), 5,
        msg = 'should return the largest element in a list')


    def test_2(self):
        # it should return the largest element in a list when there are ties
        self.assertEqual(main.get_largest_element([3, 5, 3, 1, 5]), 5,
        msg = 'should return the largest element in a list when there are ties')


    def test_3(self):
        # it should return the largest element in a list when they are all negative
        self.assertEqual(main.get_largest_element([-1, -5, -3]), -1,
        msg = 'should return the largest element in a list when they are all negative')

```

### !end-tests

### !explanation
```python
def get_largest_element(lst):
    if not lst: return 0
    return max(lst)
```
### !end-explanation

### !end-challenge

### !challenge

* type: code-snippet
* language: python3.6
* id: baa3bc1e-1a67-4a6b-a66a-72cc6e55c8b4
* title: compute_sum_of_all_elements

### !question

Write a function called "compute_sum_of_all_elements".

Given a list of numbers, "compute_sum_of_all_elements" returns the sum of all the elements in the given list.

Note: Function should return 0 if the list is empty.

```
output = compute_sum_of_all_elements([1, 2, 3])
print(output) # --> 6
```

### !end-question

### !placeholder

```python
# your code here



```

### !end-placeholder

### !tests

```python
import main
import unittest

class TestScript(unittest.TestCase):

    def test_0(self):
        # it should return a number
        self.assertIsInstance(main.compute_sum_of_all_elements([1, 2, 4]), (float, int),
        msg = 'should return a number')


    def test_1(self):
        # it return the sum of all elements
        self.assertEqual(main.compute_sum_of_all_elements([1, 2, 4]), 7,
        msg = 'return the sum of all elements')


    def test_2(self):
        # it return 0 if the passed in list is empty
        self.assertEqual(main.compute_sum_of_all_elements([]), 0,
        msg = 'return 0 if the passed in list is empty')

```

### !end-tests

### !explanation
```python
def compute_sum_of_all_elements(lst):
    if not lst: return 0
    return sum(lst)

```
### !end-explanation

### !end-challenge
