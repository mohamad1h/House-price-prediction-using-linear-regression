import numpy as np
from sklearn.linear_model import LinearRegression

#read the input parameter of the training matrix
F,N=map(int,input().split())

#storing the input values into the feature matrix X and into the label vector y
data=[]
data=np.array([list(map(float,input().split())) for _ in range(N)])
X=data[:,:-1]
y=data[:,-1]


#read the nb of rows of the prediction matrix
p=int(input())

#storing the input featur matrix into pred
pred=[]
pred=np.array([list(map(float,input().split())) for _ in range(p)])

#building the linear model
model=LinearRegression()
model.fit(X,y)

#estimating the price of the house of each row input containing the feature of the house
pred_value=model.predict(pred)

#displaying the rounded value
for i in range(p):
    print(round((pred_value[i]+0.05)*100)/100)
