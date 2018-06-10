# Quiz01
My first code
def matVec(matrix,vector): 
  """
  This function takes in a matrix with a vector and for each element in the matrix multiplies the elements of the vector and stores it in the blank matrix f. Fuction returns f.
  """
  f=[]
  for i in range(len(matrix)):
    c=[]
    for j in range(len(matrix[i])):
      for k in range(len(vector)):
        d=[]
        for l in range(len(vector[k])):
          d.append(matrix[i][j]*vector[j][k])
    c.append(d)
  return f

matrix = [[1,2,3],[3,4,5]]
vector = [2,3,4]
print (matVec(matrix,vector)) 
