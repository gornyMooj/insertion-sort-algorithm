# Insertion sort algorithm

with Python

```python
import random


def create_random_arrey(n,x,y):
    my_list = [random.randint(x, y) for i in range(n)]

    return my_list


def insertion_sort_algorithm(my_list):
    for i in range(1, len(my_list)):
        for j in range(i,0, -1):
            if my_list[j] < my_list[j-1]:
                my_list[j],my_list[j-1]= my_list[j-1],my_list[j]
            else:
                #no swaps left we can break the loop
                break

my_list = create_random_arrey(20,1,30)
print("Random list: ",my_list)

insertion_sort_algorithm(my_list)
print("Sorted list: ",my_list)
```
