Packaging Python Projects

https://packaging.python.org/en/latest/tutorials/packaging-projects/

NOTE that the project directory is different from the tutorial.
no /src/

with src you would need to run 
```
from src.example_package_co import example
```
instead



```
python3 -m pip install --upgrade pip

python3 -m pip install --upgrade build
python3 -m build

python3 -m pip install --upgrade twine
python3 -m twine upload --repository testpypi dist/*
python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps example_package_co
python3 -m pip list
python3 -m pip uninstall example_package_co

from example_package_co import example
example.add_one(3)
```