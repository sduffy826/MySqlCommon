## Common MySql routines

This has common code.  It is meant to be imported into the appropriate python project.  In
order to do this
- This directory (MySqlCommon) should be at the same 'level' as the directory that uses it, i.e.
if you have directory 'ProjectABC' at path '/level1/level2/ProjectABC', then you should have
the code from this repo in '/level1/level2/MySqlCommon'
- Make sure you update file 'mySqlConnectionVars.py' to reflect the mysql db you want to connect to
- Copy the 'addMySqlToPath.py' code from the MySqlCommon directory into your project 
- In your code you should have
```
  from addMySqlToPath.py import *  # Does the work of adding MySqlCommon to path
  import mySqlRoutines as mySql    # Will do import (like having import ../MySqlCommon/mySqlRoutines)
  import mySqlUtils as mySqlUtils  # Import utility routines if you want
```

