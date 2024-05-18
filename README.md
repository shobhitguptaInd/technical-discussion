# technical-discussion
this is a demo repository for sharing ideas around communication


## Lesson -1 - Learning Github

* Creating technical discussion respository
* Creating a gist
* Create a notebook on collab
* Learning integration with cloud
* Python code base for sharing

##Gist
 this is a good example of kind of code I will have here [mycode](https://gist.github.com/shobhitguptaInd/1362fef3564c7706034d033a70e137d5)

##Colab
this is a notebook [mynotebook](https://github.com/shobhitguptaInd/technical-discussion/blob/5662196e4e5de5b7aeca2511ad2ef64651b0d780/technicalDocs.ipynb)

##Image
![image](https://github.com/shobhitguptaInd/technical-discussion/assets/53973923/1497220b-bb2b-4431-ae63-d5a084a42e66)

##Python Project
* MAKEFILE - Recipe of building software, available on Linux
* Tests - Functional, Integration, Load/Performance, 
* LINTING - Best Practice, Check for Bad Syntax, Catches bugs, enhances automation
* Python Virtual Environment - Isolate Python to a directory | python3 - m venv ~/.<project-dir> | dot in front of directory name makes is invisible | source ~/.<project-dir>/bin/activate
* Github Actions - SaaS|Continuous Integration| YAML based
* Continuous Integration  - Local Scaffolding with Makefile, Test, Virtual Env | Github actions to checkout code, Test, deploy
* Python project Scaffold - Github REPO Checkout
  ** Makefile
  ** requirements.txt
  ** Code
  ** Test code
  ** Virtual Env
* AWS cloud 9 environment
  ** Create SSH Key - SSH-keygen -t rsa (tip: leave all inputs blank)| CAT <public key address> | copy key and create new SSH key on github account from account settings
  ** On AWS cloud 9 env do a git clone of your github repository
  ** create all the files as above (if they do not exist) | touch Makefile | touch hello.py | touch test_hello.py | touch requirements.txt
  ** create virtual env | python 3 -m venv ~/.scaffold | activate it | source ~/.scaffold/bin/activate
  ** create Makefile - Install, format, lint, test
  ** create requirements.txt
  ** run make install file
  ** edit code
  ** run make lint
  ** run git status
  ** run git add *
