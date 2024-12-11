OVERVIEW:
-
In this project we would be deploying a to-do app, where we can add our daily day to day tasks, and edit and delete the tasks once done. And the same application would be deployed using google cloud platform for enabling public access to the application.

INSTRUCTIONS FOR SETTING UP AND RUNNING THE APPLICATION: 
-
Install Python 3.13.1 and run the execution file and complete the downloading process completely. 

In the same directory install the opensource python framework, FLASK which helps to design a scalable and flexible application. 

Choose any of the source code editors like VsCode and type all the 3 codes required for a good functioning of the website.  The file structure should look like the following :

--> main.py (backend code for flask)

--> requirements.txt (for Python dependencies like flask)

--> Procfile (for deployment on cloud platforms)

-->/Templates (html templates)

    -->Index.html
  
    --> edit.html

(additionally if css is required, then include it in another folder and name it as "static")

-->/Statics (for css and js files)

    -->styles.css

  FOR RUNNING THE ABOVE PROJECT, in the terminal run the command "python main.py". and a local host address will be generated which would lead you to the to-do functional application.

  INSTRUCTIONS/COMMANDS FOR PUSHING THE LOCAL PROJECT INTO YOUR GITHUB REPOSITORY
  -
  -Install Git in your laptop first.
  
  -Go to the folder where your project files are saved, and rightclick + "git Bash here", Git terminal will open where you need to execute the following commands
  
       -> $ git config --global user.name "Pjanavi"
       
       -> $ git config --global user.email "janavisarathy2003@gmail.com"
       
       -> $ git init
       
       -> $ git commit -am "initial commit"
       
       -> $ git add .
       
       -> $ git remote add origin https://github.com/Pjanavi/cloud-deploy.git  [Insert your github public repository link]
       
       -> $ git push origin main

INSTRUCTIONS FOR DEPLOYING THE GITHUB REPO ON A PUBLIC SERVER, IN THIS CASE IT'S YOUR GOOGLE ACCOUNT USING "CLOUD RUN" 
-
-Login to your google cloud account. 

-Go to Google Cloud Console --> "Cloud Run" --> "Connect Repo" --> Continously deploy from a Repository --> "Setup with cloud build."

        --> In "setup with cloud build" choose your github profile and click on authenticate further choose the repository you want to deploy and click on --> NEXT
        
        --> In Build Configurations: -->choose main branch (if there is only one branch in your github repo and main branch is a default branch) and choose -->Go, Nodejs, Python file.
        
             -->Entry point would be your "python main.py"  and click on "SAVE"
             
        --> Service name would be the same name as your repository and select region--> Mumbai(Asia)
        
        --> Enable "Allow unauthenticated invocations" as there's no confidential information as of now in this project
        
        --> Change the minimum instances to 1
        
        --> let the remaining options be the default chose itself. 
        
        --> click on "CREATE"
        
        --> Now the project will be succesfully deployed and a public url will be generated
        
        --> IN THIS PROJECT THE FINAL PUBLIC URL GENERATED IS : "https://cloud-deployy-1077873054506.asia-south1.run.app/"


PROJECT OUTPUT 
-
https://cloud-deployy-1077873054506.asia-south1.run.app/
        
      

  

    
