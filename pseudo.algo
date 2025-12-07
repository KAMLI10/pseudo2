//Problem 1
ALGORITHM SUM_DISTINCT_ELEMENTS
VAR
  i, j, sum : INTEGER
  found : BOOLEAN

BEGIN
  sum = 0

  // Check unique elements from set1
  For i = 1 to n1 do
      found = false
      For j = 1 to n2 do
          If set1[i] == set2[j] then
              found = true
          EndIf
      EndFor
      If found == false then
           sum = sum + set1[i]
      EndIf
  EndFor

  // Check unique elements from set2
  For i = 1 to n2 do
      found = false
      For j = 1 to n1 do
          If set2[i] == set1[j] then
              found = true
          EndIf
      EndFor
      If found == false then
          sum = sum + set2[i]
      EndIf
  EndFor

  Write ("Sum of distinct elements = ", sum)
END




// Problem 2
ALGORITHM DOT_PRODUCT_AND_ORTHOGONALITY
VAR
  n, i, j, num_pairs : INTEGER
  v1, v2 : ARRAY[1..n] OF REAL
  v1,v2 : ARRAY_OF REAL[n];
  ps : REAL

// Function to calculate dot product of two vectors
FUNCTION dot_product(vector1, vector2, size)
VAR
  sum : REAL
  k : INTEGER
BEGIN
  sum = 0
  For k = 1 to size do
      sum = sum + vector1[k] * vector2[k]
  EndFor
  RETURN sum
END

BEGIN
  // Input: number of vector pairs
  Write ("Enter number of vector pairs: ")
  Read (num_pairs)

  For i = 1 to num_pairs do
      Write ("Enter size of vectors for pair ", i, ": ")
      Read (n)

      // Input elements of vector v1
      For j = 1 to n do
          Write ("Enter v1[", j, "]: ")
          Read (v1[j])
      EndFor

      // Input elements of vector v2
      For j = 1 to n do
          Write ("Enter v2[", j, "]: ")
          Read (v2[j])
      EndFor

      // Calculate dot product
      ps = dot_product(v1, v2, n)

      // Check orthogonality
      If ps == 0 then
          Write ("Pair ", i, " vectors are orthogonal.")
      Else
          Write ("Pair ", i, " vectors are NOT orthogonal.")
      EndIf
  EndFor
END
