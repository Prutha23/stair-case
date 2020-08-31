# stair-case
In input, an N*M/ N*N  matrix is given. We have to traverse and print elements of the matrix in the staircase pattern i.e. first right, then the bottom, then again right, and so on. You can not visit one element more than once. Once you reach the last element of the matrix traverse back to the 1st column and then to the first row. This won’t be possible in the N*M matrix. I had to write one function which takes care of all 3 possibilities. 
Consider the following 3 different scenarios :
N > M:
Input : 1 2 3 4
	5 6 7 8
	9 10 11 12
Output : 1 2 6 7 11 12. 
Explanation: 1 → 2
		             ↓
	               6 → 7
                     ↓
                     11 → 12
N < M:
Input: 1 2 3
	4 5 6
	7 8 9
	10 11 12
Output: 1 2 5 6 9
Explanation: 1 → 2
	               ↓
	               5 → 6 
		                 ↓
		                 9
                     
N = M:
Input : 1  2  3  4
	      5  6  7  8
        9 10 11 12
	      13 14 15 16
Output: 1 2 6 7 11 12 16 15 14 13 9 5 
Explanation: 1 → 2
		             ↓
	          5    6 → 7
            ↑        ↓
            9        11 → 12
            ↑              ↓
            13 ← 14 ← 15 ← 16
