# QUESTIONS
- I created a venv but what is the usual approach? devcontainer? Also, is there a requirement.txt? I saw requirements-doc.txt
  - Not a fan of devcontainer
  - depends, pyenv is also a good choice
- Curious about the reason to import "from pandas import DataFrame" rather than using standard pd.DataFrame
  - style reasons
  - linting (black)

- Can't run zz_test.py even though all libs are installed in the venv...
- In analysis builder, why does the abstract method in the ABC class have parameters? 
  - In python you can specify certain behavior in interface methods via ABC abstractmethod. In other words, when a subclass implements this method, it must accept the same parameters.
  - Union is limiting the options for the data types... could be expanded to spark
- Is df mapping to data? why change the name?
  - Actually an error, not best practice to have the concrete implementation with different parameters
- I don't get theuse of static method in data_processor.py


## NOTES
1. data.data_reader
   1. add spark option for CsvReader class ?
   2. add parquet reader class ? (might be other feature)
   3. 