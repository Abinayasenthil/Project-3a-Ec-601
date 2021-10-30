# Project-3a-Ec-601
#Unit Test for Project 2
python -m pytest
If you don’t have PyTest, it’s installed by:
python -m pip install pytest
on:
 push:
   paths:
     - "**.py"

jobs:
 Integration:
   runs-on: ${{ matrix.os }}
   strategy:
     matrix:
       os: [ubuntu-latest, macos-latest]
       python-version: [3.6, 3.7, 3.8]
   steps:
   - uses: actions/abinayasenthil@v2
   - uses: actions/setup-python@v2
     with:
       python-version: ${{ matrix.python-version }}
   - run: pip install .[tests]
   - run: pytest
import sys
def add(x:float,y:float):
return x+y
if__name__=='__main__'
x=sys.argv[1]
y=sys.argv[2]
S=add(float(x),float(y))
print(s)
import mathfun as fun
from pytest import apporx
def test_addints()
assert fun.add(1,1)=2
