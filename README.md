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
* Python Virtual Environment - Isolate Python to a directory | python3 - m venv ~/.<project-dir> / virtualenv ~/.<project-dir> | dot in front of directory name makes is invisible | source ~/.<project-dir>/bin/activate
* Github Actions - SaaS|Continuous Integration| YAML based
* Continuous Integration  - Local Scaffolding with Makefile, Test, Virtual Env | Github actions to checkout code, Test, deploy
* Python project Scaffold - Github REPO Checkout
  ** Makefile
  ** requirements.txt
  ** Code
  ** Test code
  ** Virtual Env
* AWS cloud 9 environment/Azure/GCP
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
  ** run git commit
  ** run git push
  ** App deployment - gcloud app deploy
**Continuous delivery - GCP
  ** Service: Cloud build
  ** Select Trigger - Create Trigger - Connect repository
  ** go to settings below triggers - enable app engine and service accounts
  ** Any changes commited on github will be automatically deployed on cloud


** Static website on cloud
** create a index.html page om EC2 cloud instance
** create a S3 bucket with public access
** modify properties of the bcuket created to make it host a static website
** add bucket policy 

     {
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::shobhit-gupta-first/*"
        }
    ]
}
** upload index.html in the bucket
** access website link from properties>static website hosting


### Build AWS Lambda Service
** Click on AWS and create SAM application
** For HTTPS webservice
 ** Setup PEM Key -  Create key pair on EC2 (automatically downloaded on creation)
 ** upload pem key file on Cloud 9
 ** Create security gorup on port 22 and 80 -> On EC2 instance -> Security groups -> new security group with 2 inbound rules for port 22 and 80 on 0.0.0.0/0
 ** Create Spot -> EC2->spot request-> select AMR-Linux 2 -> security group and Key pair created.
 ** Appropriatly name SSH instance->connect-> get SSH connecting details-> connect with cloud 9-> update software using commands below once connected
  ** sudo yum update -y  ** sudo yum install -y httpd  ** sudo systemctl start  httpd
 ** Add content to web location -> sudo usermod -a -G apache ec2-user -> sudo chown -R ec2-user:apache /var/www -> sudo chmod 2775  /var/www && find /var/www -type d -exec sudo chmod 2775 {}
\; find /var/www -type f -exec  sudo chmod 0664 {} \; create index.html in /var/www/html -> sudo systemctl restart  httpd


### PAAS
** AWS Elastic Beanstak, GCP Google app engine , AWS App Services
** EB CLI setup

## Devops
** CI, CD, Microserices, Infrastructure as code, monitoring, communication and collaboration

### Infra as code




  

  
  
