# belly-button-challenge
Interactive Dashboards MOD 14 (week 14)

In this assignment, you will build an interactive dashboard to explore the Belly Button Biodiversity dataset Link: 'https://robdunnlab.com/projects/belly-button-biodiversity/' which catalogs the microbes that colonize human navels.

The dataset reveals that a small handful of microbial species (also called operational taxonomic units, or OTUs, in the study) were present in more than 70% of people, while the rest were relatively rare.

Goals- 
Complete the following steps:

1. Use the D3 library to read in 'samples.json' from the URL https://static.bc-edx.com/data/dl-1-2/m14/lms/starter/samples.json.
2. Create a horizontal bar chart with a dropdown menu to display the top 10 OTUs found in that individual.
    a. Use 'sample_values' as the values for the bar chart.
    b  . Use 'otu_ids' as the labels for the bar chart.
    c. Use 'otu_labels' as the hovertext for the chart.
3. Create a bubble chart that displays each sample.
    a. Use 'otu_ids' for the x values.
    b. Use 'sample_values' for the y values.
    c. Use 'sample_values' for the marker size.
    d. Use 'otu_ids' for the marker colors.
    e. Use 'otu_labels' for the text values.
4. Display the sample's metadata, i.e., an individual's demographic information.
    a. Loop through each key-value pair from the metadata JSON object and create a text string.
    b. Append an html tag with that text to the '#sample-metadata' panel.
5. Update all the plots when a new sample is selected. Additionally, you are welcome to create any layout that you would like for your dashboard.
6. Deploy your app to a free static page hosting service, such as GitHub Pages. Submit the links to your deployment and your GitHub repo. Ensure that your repository has regular commits and a thorough README.md file

Additional/Detailed Instructions

1. Filter the metadata for the object with the desired sample number
2. Use d3 to select the panel with id of `#sample-metadata`
3. Use `.html("") to clear any existing metadata
4. Inside a loop, you will need to use d3 to append new
5. tags for each key-value in the filtered metadata.
6. function to build both charts
7. Get the samples field
8. Filter the samples for the object with the desired sample number
9. Get the otu_ids, otu_labels, and sample_values
10. Build a Bubble Chart
11. Render the Bubble Chart
12. For the Bar Chart, map the otu_ids to a list of strings for your yticks
13. Build a Bar Chart
14. Render the Bar Chart
15. Get the names field
16. Use d3 to select the dropdown with id of `#selDataset`
17. Use the list of sample names to populate the select options

    Hint: Inside a loop, you will need to use d3 to append a new option for each sample name.

18. Get the first sample from the list
19. Build charts and metadata panel with the first sample
20. Function for event listener
21. Build charts and metadata panel each time a new sample is selected
22. Initialize the dashboard.
