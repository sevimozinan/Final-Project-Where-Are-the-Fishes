# Final Project - Where Are the Fishes? 

My project of Statistical Analysis Software (Rstudio) at Marmara University.

![Imgur Image](https://imgur.com/eR1jvTr.jpg)

Exploring acoustic backscatter data to find fish in the US Atlantic Ocean. 

Reflections. No, I’m not talking about contemplating your existence within the Tidyverse or understanding what that spline did to your data. I’m talking about echoes. Specifically, acoustic echoes called “backscatter.” Marine scientists use acoustic backscatter to understand the distribution of organisms in the ocean.

In this analysis, together with Sevim Ozinan, Mehtap Fil and Yasemin Hizarci we discussed wrangle active acoustic data and plotted the mean volume backscatter associated with fish with swim-bladders in relation to bathymetry (depth of the seafloor)

These acoustic data were collected from a research vessel that crossed the shelf break in the Mid-Atlantic Bight (NOAA cruise HB1103) and were preprocessed using the software, Echoview.

# Stages in this project
1. Backscatter - remote sensing in the ocean (Load the libraries)
2. What is the "shelf break"? (Clean the bottom data and then inspect the data )
3. Where ever you go, there you are (Plot the ship's track, plot the depth of the sea floor along the ship's track, arrange the plots side by side for easier viewing)
4. Here fishy, fishy, fishy... (Read in the acoustic data and then glimpse the data)
5. That's a lot of variables! (Create a list of variables to keep, select and filter the data, glimpse the cleaned acoustic data) 
6. A little more wrangling (Data prep for temporal interval join)
7. Can't go spatial? Go temporal (Function: assign Spatial_interval to bottom points that fall within Time_interval, map the track line interval value to bottom_clean)
8. Depth of an Interval (Group bottom_clean and calculate the mean depth, join the bottom intervals data to the acoustic data)
9. Putting it all together (Group bottom_clean and calculate the mean depth, join the bottom intervals data to the acoustic data)
10. So, where are the fishes? (If we assume that all the acoustic backscatter is only from fishes with swim bladders, and greater backscatter indicates higher densities of fish, where are most of the fish on this track line? Options: Shelf, Shelf Break, Offshore)

![Imgur Image](https://imgur.com/pkiy5ay.jpg)
