# Quiz01
def matVec(matrix,vector): 
  """
  This function takes in a matrix with a vector and for each element in the matrix multiplies the elements of the vector and stores it in the blank matrix f. Fuction returns f.
  """
 
  f=[0]*len(matrix)
   #This Matrix is filled with zeros with the dimensions of the matrix that we need
  for i in range(len(matrix)):
    #This is to show the length of the rows of the matrix 
    for j in range(len(matrix[i])):
      #This is to show the row and column of the elements in the matrix
      z = matrix[i][j] * vector[j]
      #This is to multiply the firs element of the matrix and the first element of the vector and so on. 
      f[i] = f[i]+z
      #Since we are multiplying [i][j] to the elements of the vectors seperatly, this is for the purpose of adding them together at the end. 
  return f
  #This returns the matrix after it has been added together

# Test Case 1
matrix = [[1,2,3],[3,4,5]]
vector = [2,3,4]
print (matVec(matrix,vector)) 
# Test Case 2
print (matVec(vector,matrix)) 
# test Case 3
print (matVec("Houston Texans",99))
