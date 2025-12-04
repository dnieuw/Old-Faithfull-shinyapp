# Old Faithful Shiny App

A classic R Shiny app demonstrating the Old Faithful geyser data, configured to run in GitHub Codespaces using the `rocker/tidyverse` Docker container.

## About

This repository contains the classic "Old Faithful" R Shiny demo app that visualizes the waiting time between eruptions of the Old Faithful geyser in Yellowstone National Park.

## Running in GitHub Codespaces

1. Click the green "Code" button on the repository page
2. Select "Open with Codespaces"
3. Create a new Codespace or select an existing one
4. Once the Codespace is ready, open a terminal and run:
   ```r
   R -e "shiny::runApp('app.R', port = 3838, host = '0.0.0.0')"
   ```
5. The app will be available on port 3838 (which will be automatically forwarded)

## Running Locally

If you have R installed with the `shiny` package:

```r
shiny::runApp('app.R')
```

## Container

This project uses the `rocker/tidyverse` Docker image, which includes R and the tidyverse packages. The devcontainer configuration automatically installs the `shiny` package when the Codespace is created.