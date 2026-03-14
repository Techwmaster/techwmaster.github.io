---
title: DevOps Best Practices
date: 2026-03-12 18:30:00 -500
categories: [DevOps]
tags: [Github,CI/CD, AWS, Automation]  # TAG names should always be lowercase
---



## Tech Stack

GitHub, AWS, AWS CLI, Python

## Step1: Create a new repo in your GitHub

Let's create a new repo in our GitHub.

Name: DevOps-Best-Practices

Description: A Recipe for a good DevOps Compliant project 

In the new GitHub repo created, let's add:
- a README file
- a .gitignore file

We will add the other files directly through our IDE by using "touch".

## Step 2: Connect to your AWS account or Cloud provider

As we will use AWS as our Cloud provider, we need to ensure we can communicate with AWS through our IDE command line.

Install AWS CLI in your system.

For Linux type system.

```Bash
$ curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install

```

For other systems, here is the references: 
https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html#getting-started-install-instructions 


## Step 3: Create a virtual environment in your IDE

Let's create a virtual environment to run our python code so the packages installation does not affect our system.

To create a Python virtual environment on Linux using the command line, follow these steps:

**Note**: Ensure `python3` and `python3-venv` are installed. On Debian/Ubuntu, install them with:  
```bash
sudo apt update && sudo apt install python3 python3-venv
```


**Create the Virtual Environment**  
Run the following command in your terminal, replacing `virtualenv` with your desired environment name:  
```bash
python3 -m venv virtualenv
```

This creates a new directory named `virtualenv` containing a fresh Python installation and isolated environment.

**Activate the Virtual Environment**  
Use this command to activate it:  
```bash
source virtualenv/bin/activate
```

After activation, your terminal prompt will change to show the environment name (e.g., `(virtualenv)`), indicating you’re now working within the isolated environment.

**Deactivate When Done**  
To exit the virtual environment, simply run:  
```bash
deactivate
```

## Step 4: Clone your repo into your IDE

Choose a local folder to save the cloned repository.
In your command line :

pwd, cd,

```bash

git clone https://github.com/Azure-Samples/cognitive-services-speech-sdk.git;

```

Open the folder in your IDE.

## step 5: Create the scaffold file in your folder

### Make sure you are working on the virtual environment !!!!!!!!!!!!

We will create an app.py, a test.py, a MakeFile and a requirements.txt file.

The app.py is our app.

The test.py will allow us to test our app.

The MakeFile is where we will store all our commands.

The requirements.txt is where all the packages are kept.


### Now our Scaffold structure should look like this:

app.py, MakeFile, README.md, requirements.txt, test.py

In the app.py 

```python
Print("hello world")
```

in the command line test by typing 

```bash
sudo python3 app.py
```

You should get in return 
```bash
Hello, World!
```

## To be Continuted