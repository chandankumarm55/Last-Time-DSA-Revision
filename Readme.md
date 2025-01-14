
```python
class Solution:
    def findThePrefixCommonArray(self, A: List[int], B: List[int]) -> List[int]:
        result = []
        seenA = set()
        seenB = set()
        
        # Iterate over both arrays
        for i in range(len(A)):
            seenA.add(A[i])  # Add current element of A to seenA
            seenB.add(B[i])  # Add current element of B to seenB
            
            # Count the common elements between seenA and seenB
            count = len(seenA & seenB)
            result.append(count)  # Append the count to result
        
        return result  # Return the result list
