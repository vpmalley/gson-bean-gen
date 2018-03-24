# gson-bean-gen
A python script to generate Java bean classes based on a sample json object.

You have a json object and you want to use [Gson] or [Jackson] to parse it? Here is a python script to create your Java classes for the beans to be parsed out of a sample json file. Clone the repo with the script and execute it, passing just the sample json file.

It also works well in complement of [retrofit] or [scribe]

## Quick and easy

#### Clone this repository

```bash
git clone https://github.com/vpmalley/gson-bean-gen.git
```

#### Copy a sample json file to the directory

```bash
cd ./gson-bean-gen
cp /path/to/sample.json .
```

#### Run the python script

```bash
chmod +x gson-bean-gen.py # make sure it is executable
./gson-bean-gen.py sample.json
```

#### Collect your Java files in beans directory

```bash
ls ./beans
```

## Customizable

You can change a few things by passing these arguments:
  
- (mandatory) sampleFile the path to the sample json file (including the extension)
- (optional) beanName the name of the top-level object. Default: the name of the json file is used
- (optional) memberVisibility the visibility of the members of the classes (private, protected, default or public). Default: private
- (optional) package the package for the generated classes. Default: com.example


## Extensible

Do not hesitate to extend the script and add a pull request to share it with everyone.


[Gson]: https://sites.google.com/site/gson/gson-user-guide
[Jackson]: http://wiki.fasterxml.com/JacksonHome
[retrofit]: http://square.github.io/retrofit/
[scribe]: https://github.com/fernandezpablo85/scribe-java
