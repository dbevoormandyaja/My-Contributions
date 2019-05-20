# Classes and their methods of Example - 2


#### 1. class FeedData(Stage)

       class FeedData(Stage):

          def __init__(self):
             print("I am happy")

          def operate(self, surround_data, config):
             print("this is working fine")

Here, the class `FeedData(Stage)` is nothing but a test class to check whether the integration of Vector Regression model into the Surround Framework is working fine or not.


#### 2. classs SVRData(SurroundData)

       class SVRData(SurroundData):
   
          def __init__(self):
           self.dta = pd.DataFrame()

          def getfunc(self):
     
             sth = 25
             return sth

         def get_data(self):
           
           self.dta = pd.read_csv('/Users/saikrishna/Documents/GitHub/Surround_AI_Suqad_2/Arima/arima/data/Apple_Data_300.csv')
           

**Pandas** has been imported as `pd`. The library **pandas** stands for "Python Data Analysis Library". **DataFrame** is  two-dimensional labelled data structure with columns of potentially different types, like a spreadsheet or SQL table, or a dict of Series objects. It is generally the most commonly used **pandas** object.

