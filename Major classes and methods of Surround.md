### Classes

#### 1. class Surround(ABC):

class Surround(ABC):

    def __init__(self, surround_stages=None, module=None):
        self.surround_stages = surround_stages

#### 2. class Wrapper():

class Wrapper():
    def __init__(self, surround, type_of_uploaded_object=None):
        self.surround = surround
        self.actual_type_of_uploaded_object = None
        if type_of_uploaded_object:
            self.type_of_uploaded_object = type_of_uploaded_object
        else:
            self.type_of_uploaded_object = AllowedTypes.JSON
        self.surround.init_stages()

#### 3. class AllowedTypes(Enum):

class AllowedTypes(Enum):
    JSON = ["application/json"]
    FILE = ["file"]


#### 4. class Stage(ABC):

class Stage(ABC):
    def dump_output(self, surround_data, config):
     """Dump the output of each stage.
        :param surround_data: Stores intermediate data from each stage in the pipeline
        :type surround_data: Instance or child of the SurroundData class
        :param config: Config of the pipeline
        :type config: <class 'surround.config.Config'>
        """

    @abstractmethod
    def operate(self, surround_data, config):
        """A stage in a surround pipeline.
        :param surround_data: Stores intermediate data from each stage in the pipeline
        :type surround_data: Instance or child of the SurroundData class
        :param config: Contains the settings for each stage
        :type config: <class 'surround.config.Config'>
        """

    def init_stage(self, config):
        """Initialise stage with some data
        :param config: Contains the settings for each stage
        :type config: <class 'surround.config.Config'>
        """


### Methods

stage.split(".")

".".join()

.append()

.dump_output()

datetime.now()
