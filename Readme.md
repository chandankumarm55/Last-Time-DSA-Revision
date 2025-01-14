class Solution:
    def findThePrefixCommonArray(self, A: List[int], B: List[int]) -> List[int]:
        result =[]
        seenA = set()
        seenB = set()
        for i in range(len(A)):
            seenA.add(A[i])
            seenB.add(B[i])
            count = len(seenA & seenB)
            result.append(count)
        return result 
    this above program solve we can using the sets and operations and return the element which present in both the set and also length
