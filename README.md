# gson-bean-gen
A python script to generate Java bean classes based on a sample json object.

## Quick and easy

1. clone this repository

    git clone https://github.com/vpmalley/gson-bean-gen.git

2. copy a sample json file to the directory

    cd ./gson-bean-gen
    cp /path/to/sample.json .

3. run the python script

    ./gson-bean-gen.py sample.json MyBean

4. Collect your Java files in beans directory

   ls ./beans
   
   
## Customizable

You can change a few things by passing these arguments:
  
- (mandatory) sampleFile the path to the sample json file (including the extension)
- (optional) beanName the name of the top-level object. Default: the name of the json file is used
- (optional) memberVisibility the visibility of the members of the classes (private, protected, default or public). Default: private
- (optional) package the package for the generated classes. Default: com.example


## Extensible

Do not hesitate to extend the script and add a pull request to share it with everyone.
