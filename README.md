# Biostat777 Project 3 Part 1



## Project Description
See: https://www.stephaniehicks.com/jhustatprogramming2023/projects/2023-11-28-project-3/

Note: This is an original package I developed! Hence, there is no Github link to the origin destination



## Package
STTileMaker

Website: XXX



## Author/Creator
Caleb Hallinan



## Goal of Package
Create image tiles of each spot in a H&E image Spatial Transcriptomics Dataset



## Functions
- STTileMaker_read_data() - reads in the data that contains the image, gene expression, and various other variables

- STTileMaker_make_tiles() - creates the tiles from the H&E image at each spot

- STTileMaker_plot_tile() - a quality check function that plots a single tile to confirm it works!




## Example

#### read in data

data = STTileMaker_read_data(here::here("data/f12hr_140_processed/outs/"))

####make tiles

tiles = STTileMaker_make_tiles(data)

#### check to see it works

STTileMaker_plot_tile(tiles, 1)
STTileMaker_plot_tile(tiles, 100)



## How to Download

#### Please run the following commands in your R terminal to install and use these functions

remotes::install_github(repo = "jhu-statprogramming-fall-2023/biostat777-project3-part1-calebhallinan")

library(STTileMaker)

#### OR

Clone this repository and build the package from within R



## 5 Website Customizations



## Notes/Thoughts:

- This was a cool project! I am glad I was able to create a function that I can use for my research :)
