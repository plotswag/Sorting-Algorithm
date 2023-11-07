# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Jeevanesh
RegisterNumber:212222243002 
'''
def selection_sort(nums):
    for i in range(len(nums)):
        low=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[low]:
                low=j
        nums[i],nums[low]=nums[low],nums[i]
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)

```
ii)	#Insertion Sort
``` 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Jeevanesh
RegisterNumber:212222243002 
'''
def insertion_sort(nums):
    for i in range(len(nums)):
        item=nums[i]
        j=i-1
        while j>=0 and nums[j] > item:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=item    
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)
```
## Output:
![image](https://github.com/plotswag/Sorting-Algorithm/assets/145822344/97d4220f-d329-4b30-9574-5d403ce7103a)
![image](https://github.com/plotswag/Sorting-Algorithm/assets/145822344/8c8f744b-50d6-48ce-9ed2-1c888e029a88)
## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
