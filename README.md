# Merge-Discontinuous-Time-Ranges
You are given an array of time ranges representing when a system was active.
Each range is an array [start, end) where both start and end are UNIX timestamps in milliseconds.

1. The range includes start but excludes end.
Example: [0, 5) → covers timestamps 0, 1, 2, 3, 4

3. Ranges may overlap or touch.

3. Some may be separated by small gaps.

4. Gaps smaller than or equal to the threshold (in milliseconds) should be treated as continuous and merged.
Your task is to implement a Node.js module that merges all such ranges into sorted, non-overlapping intervals.
---------------------------
/**
 * Merges discontinuous time ranges within a given threshold.
 *
 * @param {Array<[number, number]>} ranges - Array of [start, end) ranges (unsorted, may overlap)
 * @param {number} threshold - Max gap (in ms) allowed between ranges to still be merged
 * @returns {Array<[number, number]>} - Sorted, non-overlapping merged ranges
 */
const mergeTimeRanges = (ranges, threshold) => {
  // Implementation
};

module.exports = {
  mergeTimeRanges,
};

--------------
merge-time-ranges/
├── my-module.js        # Contains the mergeTimeRanges function
├── test.js             # Test file with example inputs and outputs
├── package.json        # Metadata for Node.js module
└── README.md           # Project documentation
