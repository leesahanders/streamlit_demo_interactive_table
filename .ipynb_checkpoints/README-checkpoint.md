[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/streamlit/example-app-interactive-table/main)

# 🖱️ Interactive table app

This app shows how you can use the [streamlit-aggrid](https://github.com/PablocFonseca/streamlit-aggrid) Streamlit component in an interactive way so as to display additional content based on user click.

<img src ="https://user-images.githubusercontent.com/7164864/152407708-1f3394bd-a683-4520-8677-c94e3872bb22.png" width="400px"></img>

### Questions? Comments?

Please ask in the [Streamlit community](https://discuss.streamlit.io).

# Workbench

Referencing [here](https://solutions.rstudio.com/python/jupyter/). 

First clone the repository:
git clone https://github.com/streamlit/<app-name>
    
Create a virtual environment
`/opt/python/3.10.4/bin/python -m venv venv`

(You can list python versions with `which python`)
    
Active the virtual environment
`. ./venv/bin/activate`
    
Register your virtual environment as a jupyter kernel
```
(venv)$ python -m pip install ipykernel
(venv)$ python -m ipykernel install --name "<PROJECT-NAME>" --user
```

For example: `python -m ipykernel install --name "streamlit_demo_interactive_table" --user`
    
In the Jupyter UI, navigate to your project folder and create a new notebook using your newly registered kernel. If your kernel does not show up, you may need to refresh the page in your browser.

You should see something like: 
Installed kernelspec streamlit_demo_interactive_table in /usr/home/lisa.anders/.local/share/jupyter/kernels/streamlit_demo_interactive_table
    
Streamlit will need to be installed: 
`pip install streamlit`
    
Test streamlit: 
`streamlit hello`

Install any required dependencies. Test the app locally:
`streamlit run <app-name>/streamlit_app.py`
For example: `streamlit run streamlit_demo_interactive_table/streamlit_app.py`

Over time, you may build up lots of available Jupyter kernels. These can be managed from the command line. For example, to list all the available kernels:
`$ jupyter kernelspec list`
    
Or to remove an old unused kernel:
`$ jupyter kernelspec remove <KERNEL-NAME>`
    
# Publishing 

Instructions from [here](https://docs.rstudio.com/connect/user/streamlit/). 

rsconnect will need to be installed: 
`pip install rsconnect-python`
    
Then deploy to RStudio Connect:
`rsconnect deploy streamlit -n <saved server name> --entrypoint streamlit_app.py <app-name>/`
For example: `rsconnect deploy streamlit -n <saved server name> --entrypoint streamlit_app.py streamlit_demo_interactive_table/`

Some debugging references: 
    
 - [Streamlit Tutorial: How to Deploy Streamlit Apps on RStudio Connect](https://www.r-bloggers.com/2022/02/streamlit-tutorial-how-to-deploy-streamlit-apps-on-rstudio-connect/)
 - [Using Python with RStudio Team](https://www.youtube.com/watch?v=o36425S1-VU)
 - [Streamlit article on Solutions](https://docs.rstudio.com/connect/user/streamlit/)
 - 

