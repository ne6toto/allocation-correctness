## allocation-correctness
Verifying the correctness of allocations serving as solutions ot the Social Golfer Problem and Social Golfer Problem with Adjacent Group Sizes

# How to use
To check a single file run check_correctness.py. You will be prompted to enter the name of the file containing the allocation to be checked. The file must be in the same directory as the python script.

To perform a batch verification of a number of allocations, use check_all.py. The script checks all .txt files in the current folder and all of its subfolders.

# Allocation naming convention
In order for a script to check an allocation, it must know what the allocation is supposed to be. To achieve this, the filename must follow the following rules:
1. Files are named "allocation_v_(k)_i.txt" or "allocation_v_(k1,k2)_i.txt" where
- v is the number of participants in the allocation
- k is the number of participants in each group if all groups have the same size, or k1 and k2 are the number of participant each groups if the groups have two different sizes
- i is the index of the allocation, should more than one way of allocation participants exist for the same values of v and k. This index is not used in any way by the correctness checking algorithm.