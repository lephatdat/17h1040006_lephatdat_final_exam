# 17h1040006_lephatdat_final_exam
final exam

The sorting algorithm

def bubble_sort(nums):
    swapped = True
    while swapped:
        swapped = False
        for i in range(len(nums) - 1):
            if nums[i] > nums[i + 1]:
                # Swap the elements
                nums[i], nums[i + 1] = nums[i + 1], nums[i]
                # Set the flag to True so we'll loop again
                swapped = True
def selection_sort(num):
    for i in range(len(num)):

        # Find the minimum element in remaining
        # unsorted array
        min_idx = i
        for j in range(i + 1, len(num)):
            if num[min_idx] > num[j]:
                min_idx = j

                # Swap the found minimum element with
        # the first element
                num[i], num[min_idx] = num[min_idx], num[i]
