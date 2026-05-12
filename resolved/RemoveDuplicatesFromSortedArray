# Topic
- List

## Author
- Michael Spazzini


## Link
https://leetcode.com/problems/remove-duplicates-from-sorted-array/solutions/8206250/sorted-ottimale-by-spamic-55vb

# Code

## Soluzione 1 - ottimale
Questo algoritmo usa la tecnica dei two pointers per rimuovere i duplicati da un array ordinato in-place. Il puntatore i scorre l’array, mentre pos indica dove salvare il prossimo elemento unico. Quando l’elemento corrente è diverso dall’ultimo valore unico trovato, viene copiato in nums[pos] e pos viene incrementato. Alla fine, i primi pos elementi dell’array contengono tutti i valori unici in ordine. 

La complessità è O(n) in tempo e O(1) in spazio.
- Runtime: 3 ms
- Memory: 20.57 MB

```python3 []
class Solution:
    def removeDuplicates(self, nums: List[int]) -> int:
        
        pos = 1
        for i in range (1, len(nums)):
            if nums[i] != nums[pos-1]:
                nums[pos] = nums[i]
                pos +=1

        return pos

```

## Soluzione 2 - poco ottimale
- Runtime: 137 ms
- Memory: 20.39 MB

```python3 []
class Solution:
    def removeDuplicates(self, nums: List[int]) -> int:
        n = len(nums)
        i = 0
        count=n
        while i < n-1:
            if nums[i] == nums[i+1] or nums[i] == nums[i-1]:
                nums.remove(nums[i])
                nums.append("_")
                count -=1
                continue
            if nums[i+1] == "_":
                break
            i+=1
        
        return count

```