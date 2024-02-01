# Max-Diagonal-Sum
You are given a matrix of  size n x n initially all filled with 0. You can replace at most k 0's in the matrix with 1's. Your task is to find the maximum diagonal sum .

def max_diagonal_sum(n, k):
    replacements_main_diag = min(n, k)

    k -= replacements_main_diag

    replacements_other_diag = min(n, k)

    sum_main_diag = replacements_main_diag

    sum_other_diag = replacements_other_diag

    max_diagonal_sum = sum_main_diag + sum_other_diag
    return max_diagonal_sum

n, k = map(int, input().split())
result = max_diagonal_sum(n, k)
print(result)
