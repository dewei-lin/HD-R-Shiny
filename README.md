# HD R Shiny App

You can view this **R Shiny app** online on **ShinyApps.io**:

🔗 **[Live App Link](https://dewei-lin.shinyapps.io/survival_compare/)**

## About This App

This app provides an interactive way to explore **survival probability models** using the **Langbehn 2004** and **CAP** methods. Users can:

- Adjust parameters dynamically using sliders.
- Compare survival probability models visually.
- View 3D interactive plots rendered with **Plotly**.

## How to Run Locally

To run this app on your local machine, follow these steps:

1. **Clone this repository:**
   ```bash
   git clone git@github.com:dewei-lin/HD-R-Shiny.git
   cd HD-R-Shiny
2. **Install required R packages**
Open R and install the necessary packages if they are not already installed:

```r
install.packages(c("shiny", "plotly", "ggplot2"))


3. Run the app in R
In R, navigate to the app directory and launch the Shiny app:

```r
shiny::runApp("survival_compare/app")
The app should now open in your default web browser.
