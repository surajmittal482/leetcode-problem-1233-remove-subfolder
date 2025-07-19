# leetcode-problem-1233-remove-subfolder
## Problem: Remove Sub-Folders from the Filesystem  🔗 [LeetCode Problem Link](https://leetcode.com/problems/remove-sub-folders-from-the-filesystem/)


### ✅ Approach:
1. **Sort the folder paths lexicographically.**
2. Use a **stack** to track the most recent top-level folder.
3. For each folder:
   - If it **does not start with** the top folder + `/`, it's a new top-level folder → Add it to the result.
   - Otherwise, it's a subfolder → Skip it.

### 🕒 Time Complexity:
- `O(N log N + N * L)`
  - `N` = number of folders
  - `L` = average length of folder path

### 📦 Space Complexity:
- `O(N)` for storing the result and stack


