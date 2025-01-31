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
   ```

3. **Run the app in R**
In R, navigate to the app directory and launch the Shiny app:

   ```r
   shiny::runApp("survival_compare/app")
   ```
The app should now open in your default web browser.

## Some comments and thoughts

1. As you might know R has a function to draw a surface and it is often helpful for 3D visualization. However, I found it not functioning well in our case, so I decided to draw discrete 3D plot and try to smooth the plane;
2. As we discussed, different models can have a) different number of variables b) more than 3 variables, each of which leads to inconsistency in visualization. In a), when one variable is used in model A while not B, what values of this variable do we input for B? In b), what are we going to do if we are exceeding dimensions of 3? Do we want to actually go backward to 2D?
3. As you might know, different models use different datasets, how do we account for the range of each variable being different? Do we extrapolate or do we take the intersection?
