# Merge-Intervals
Given an array of intervals intervals where intervals[i] = [start, end], merge all overlapping intervals and return an array of the non-overlapping intervals that cover all the intervals in the input.
Explanation:
Sorting:

The intervals are sorted based on their start times using Arrays.sort with a custom comparator.
Merge Process:

Start with the first interval.
For each subsequent interval:
If it overlaps with the current interval, merge them by updating the end time of the current interval.
If it doesn’t overlap, add the current interval to the list and move to the next one.
Return Result:

Convert the List<int[]> to a 2D array using toArray().
