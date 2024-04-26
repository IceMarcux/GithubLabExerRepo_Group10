def median(numbers):

    sorted_numbers = sorted(numbers)

    length = len(numbers)
    if length % 2 == 0:

        mid = length // 2
        return (sorted_numbers[mid-1] + sorted_numbers[mid]) / 2
    else:

        mid = length // 2
        return sorted_numbers[mid]


def mode(numbers):

    counts = {}
    for number in numbers:
        if number in counts:
            counts[number] += 1
        else:
            counts[number] = 1

    max_count = max(counts.values())
    modes = [number for number, count in counts.items() if count == max_count]

    return modes[0]


def mean(numbers):

    total = sum(numbers)

    count = len(numbers)

    return total / count

numbers = [1, 2, 3, 4, 5, 5, 5, 6, 6, 7, 7, 8, 8, 9, 9]
print('Median: ' + str(median(numbers)))  # Output: 6
print('Mode: ' + str(mode(numbers)))      # Output: 5
print('Mean: ' + str(mean(numbers)))      # Output: 5.666666666666667


