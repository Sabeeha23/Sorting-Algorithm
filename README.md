Selection sort and Insertion sort
Aim:
To write a program to perform selection sort and insertion sort using python programming.

Equipment’s required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Moodle-Code Runner

Algorithm:
Selection Sort Algorithm:
Set the first unsorted element as the minimum
For each of the unsorted elements, check if the element < current minimum.
If yes, set the element as the new minimum.
Swap minimum with first unsorted position.
Repeat the steps 2 and 3 for all the elements in the array.

Insertion Sort Algorithm:
Set the first element as sorted element j.
For each unsorted element X, check if current sorted element j >X.
If yes, move sorted element to the right by 1.
Break the loop and insert X.
Repeat the steps 2 to 4 for sorting all the elements in the array.

Program:
i) #Selection Sort

''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Sabeeha Shaik
RegisterNumber: 23012003
'''
def selection_sort(nums):
    for i in range(len(nums)):
        low=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[low]:
                low=j
        nums[i],nums[low]=nums[low],nums[i]
    print(nums)
    
list_of_nums = eval(input())
selection_sort(list_of_nums)


ii) #Insertion Sort

''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Sabeeha Shaik
RegisterNumber: 23012003
'''
def insertion_sort(nums):
    for i in range(1,len(nums)):
        insert=nums[i]
        j=i-1
        while j>=0 and nums[j]>insert:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=insert
    print(nums)
    
    
    
list_of_nums = eval(input())
insertion_sort(list_of_nums)


Output:
![Alt text](<Screenshot 2023-12-02 110020.png>)
![Alt text](<Screenshot 2023-12-02 110020-1.png>)

Result:
Thus the program is written to perform selection sort and insertion sort using python programming
