[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/streamlit/example-app-interactive-table/main)

# 🖱️ Interactive table app

This app shows how you can use the [streamlit-aggrid](https://github.com/PablocFonseca/streamlit-aggrid) Streamlit component in an interactive way so as to display additional content based on user click.

<img src ="https://user-images.githubusercontent.com/7164864/152407708-1f3394bd-a683-4520-8677-c94e3872bb22.png" width="400px"></img>

### Questions? Comments?

Please ask in the [Streamlit community](https://discuss.streamlit.io).


# Publishing 

Instructions from [here](https://docs.rstudio.com/connect/user/streamlit/). 

To deploy one of these examples, first clone the repository:
git clone https://github.com/streamlit/<app-name>

Install any required dependencies. Test the app locally:
streamlit run <app-name>/streamlit_app.py

Then deploy to RStudio Connect:
rsconnect deploy streamlit -n <saved server name> --entrypoint streamlit_app.py <app-name>/



