# GetVar

## Motivation

PSCAD/EMTDC exports its variables in a .out file which contain ten variables plus the column with the simulation time. If your project has more than 10 variables, another .out file will be created, in order to fit them all. PSCAD/EMTDC also creates a .inf file with the name of the variables and its order in the .out files, once these files does not have a header. It may be boring to check which column belongs to each variable and also open each .out file to import these variables to your python/MATLAB etc project. 

__________________

## Description

In order to solve this problem, this package was created: by using it, one can read all of the .out files, storage its variables and also create a .csv file with all the columns and header in a unique file.

The class PSCADVar import all the variables data from the output of both programs simulations and returns it in a object.

PSCADVar reads data from .out files: just give the .INF path as argument

### Parameters

**INF_path:** str, mandatory. 

 - It's the path of the .inf file

**writecsv:** bool, optional. Default: True

 - Creates a .CSV file with all the .OUT variables and a header. 

**delout:**   bool, optional. Default: False

 - Deletes the .OUT files once they were already read

___________________

**License**

MIT License
Copyright (c) 2020 Luis Arthur Novais Haddad


Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:


The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.


THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.