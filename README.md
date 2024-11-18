# cintel-05-cintel
Cintel Project 5
Melissa Stone Rogers, [GitHub](https://github.com/meldstonerogers/cintel-05-cintel)

## Introduction
Professional project using python, shiny, and reactive.calc function to publish a reactive shiny app with continuous intelligence. 
Commands were used on a Mac machine running zsh. Project was guided by the following respository's by Dr. Denise Case: [basic app](https://github.com/denisecase/cintel-05-cintel-basic), [fancy app](https://github.com/denisecase/cintel-05-cintel-fancy), and [final CI app](https://github.com/denisecase/cintel-05-cintel).  


## Set and Dependency Management 
Create project repository in Github. Create a requirements.txt and .gitignore file for Python code. Add the following to your requirements.txt: 
- faicons 
- pandas
- pyarrow
- plotly
- scipy
- shiny
- shinylive 
- shinywidgets 

### Clone repository to your machine
```
git clone project.url
```
Verify Python version of Python 3
```
python3 --version

```
```
python3 -m venv venv
source venv/bin/activate
```
## Install required packages and dependencies into virtual enviornment

Install VS Code Extension for Shiny if you have not done so already.

Install required packages and dependencies. 
```
pip install -r requirements.txt
```
Freeze dependencies to requirements.txt  
```
python3 -m pip freeze > requirements.txt
```

### Initial Project Save
```
git add .
git commit -m "initial"                         
git push origin main
```
### Start and Complete Project 
Follow instructions within Dr. Case's GitHub repositories: [basic app](https://github.com/denisecase/cintel-05-cintel-basic); [fancy app](https://github.com/denisecase/cintel-05-cintel-fancy); [final CI app](https://github.com/denisecase/cintel-05-cintel), and other course content provided. 

#### Troubleshooting
Using the following code, I attempted to run my Shiny app within a web browser. 
```
shiny run --reload --launch-browser penguins/app.py
```

I got numerous errors and my app would not run and launch. Thanks to dilligent colleagues within the NWSU's Continuous Intelligence course, the following troubleshooting was noted. To successfully launch my Shiny app, I downgraded websockets to version 10.4 from 14.0 using the following code.
```
pip install websockets==10.4
```

Once completed, I was able to successfully run my Shiny app within a web browser with the initial code provided above.

## Complete Your Project
Save your project and push back to your repository. 
```
git add .
git commit -m "final"                         
git push origin main
```
