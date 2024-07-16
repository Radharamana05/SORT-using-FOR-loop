# SORT-using-FOR-loop
# python program to sort with using for loop.
def custom_sort(input_list):
    n = len(input_list)
    for i in range(n):
        for j in range(0, n-i-1):
            if input_list[j] > input_list[j+1]:
                input_list[j], input_list[j+1] = input_list[j+1], input_list[j]
input_list = input("Enter a list of numbers separated by spaces: ").split()
input_list = [int(x) for x in input_list] 
custom_sort(input_list)

print("Sorted list:", input_list)


# output:
Enter a list of numbers separated by spaces: 2 77 43 100 65 22 597 223 5422 675 10034 6 11
Sorted list: [2, 6, 11, 22, 43, 65, 77, 100, 223, 597, 675, 5422, 10034]
