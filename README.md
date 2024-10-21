def cumulative_sum(*args):
    total_sum = 0
    cumulative_sums = []
    
    for number in args:
        total_sum += number
        # Calculate the cumulative sum up to the current number
        cumulative_sum = sum(range(1, number + 1))
        cumulative_sums.append(cumulative_sum)
    
    return total_sum, cumulative_sums

# Example usage
result_sum, result_cumulative_sums = cumulative_sum(4, 5, 10)
print("Total Sum:", result_sum)
print("Cumulative Sums:", result_cumulative_sums)
Total Sum: 19
Cumulative Sums: [10, 15, 55]
For 4: 1 + 2 + 3 + 4 = 10For 5: 1 + 2 + 3 + 4 + 5 = 15For 10: 1 + 2 + ... + 10 = 55
