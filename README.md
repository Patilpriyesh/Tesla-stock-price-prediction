# Tesla-stock-price-prediction
Tesla stock price prediction using Python and machine learning model
Import required libraries: pandas, numpy, matplotlib.pyplot, chart_studio.plotly, plotly.graph_objs.
read the file: tesla = pd.read_csv('file_name.csv')
print the file: tesla.head()
describe the file: tesla.describe()
plot(box plot) the tesla file: tesla[['Open','High','Low','Close','Adj Close']].plot(kind='box')
set the layout, add date,title, and required items.
plot the tesla price prediction : #plotting offline by using iplot(plot)


# Building the regression model
from sklearn.model_selection import train_test_split

#For preprocessing
from sklearn.preprocessing import MinMaxScaler
from sklearn.preprocessing import StandardScaler

#For model evaluation
from sklearn.metrics import mean_squared_error as mse
from sklearn.metrics import r2_score

#Split the data into train and test sets
# Feature scaling
scaler = StandardScaler().fit(X_train)
from sklearn.linear_model import LinearRegression
#Creating a linear model
#Plot actual and predicted values for train dataset
iplot(plot2)
#Calculate scores for model evaluation

Metric           Train                Test        
r2_score  0.8658871776828707	0.8610649253244574
MSE       1821.3833862936174	1780.987539418845

# THE R2_SCORE IN TRAIN DATA THAT IS 86.58%

# THE R2_SCORE IN TEST DATA THAT IS 86.10%

# THE MEAN SQUARED ERROR IN TRAIN DATA IS 1821.38 

# THE MEAN SQUARED ERROR IN TEST DATA IS 1780.98
