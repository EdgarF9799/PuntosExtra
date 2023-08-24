# PuntosExtra


1) Create a class in a new module inside folder called utilities.

##In the custom_logging.py file, create the class.

  ```bash
import log

class CustomLogger:
     def __init__(self, name):
         self.logger = logging.getLogger(name)
         # Configure here your registration options according to your needs
         # Example: self.logger.setLevel(logging.DEBUG)

     def log(self, message):
         self.logger.info(message)
  ```

You can import and use the CustomLogger class from any file in your project, as long as the import path is correct.

For example, if you want to use the class in the main.py file inside the "api" folder, you can do the following:

  ```bash
from utilities.custom_logging import CustomLogger

logger = CustomLogger("my_logger")
logger.log("This is a log message.")
  ```

Make sure that the custom_logging.py file contains the class definition and, if necessary, set the logging options according to your needs. You can then import and use the CustomLogger class from anywhere in your project, as long as the import path is correct.
