# Classes and their methods of Example - 2

#### 1. class FeedData(Stage)

       class FeedData(Stage):

          def __init__(self):
             print("I am happy")

          def operate(self, surround_data, config):
             print("this is working fine")


The class `FeedData(Stage)`  is to input the data to the model/framework by reading the data file `Apple_Data_300.csv`.

The method `__init__(self)` is dependent on the class `FeedData(Stage)`


#### 2. classs SVRData(SurroundData)

       class SVRData(SurroundData):
   
          def __init__(self):
           self.dta = pd.DataFrame()

          def getfunc(self):
     
             sth = 25
             return sth

         def get_data(self):
           
           self.dta = pd.read_csv('/Users/saikrishna/Documents/GitHub/Surround_AI_Suqad_2/Arima/arima/data/Apple_Data_300.csv')

