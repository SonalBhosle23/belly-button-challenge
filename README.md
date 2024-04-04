# belly-button-challenge
Module 14 Challenge 
# Belly Button Biodiversity Dashboard

## Background

In this assignment, you will build an interactive dashboard to explore the Belly Button Biodiversity dataset, which catalogues the microbes that colonize human navels.

The dataset reveals that a small handful of microbial species (also called operational taxonomic units, or OTUs, in the study) were present in more than 70% of people, while the rest were relatively rare.

## Getting Started

### Repository Setup
1. Create a new repository for this project called belly-button-challenge. Do not add this Challenge to an existing repository.
2. Clone the new repository to your computer.
3. Inside your local git repository, copy the files from the StarterCode folder contained within the Module 14 Challenge zip file. (i.e., index.html, samples.json, and the static folder).
    - Note: You will not be required to access the samples.json file locally, but it is provided for reference.
4. Push the above changes to GitHub.
5. Deploy the new repository to GitHub Pages.
## buildMetadata Function
The `buildMetadata` function is responsible for displaying metadata information for a given sample ID. It fetches metadata from an external JSON file and populates the metadata panel in the HTML with key-value pairs. It follows these steps:
- Asynchronously fetches metadata from an external JSON file using D3.js.
- Extracts the 'metadata' array from the fetched data.
- Filters the 'metadata' array based on the provided 'sample' ID.
- Clears any existing metadata in the panel.
- Iterates through each key-value pair in the metadata and appends them as <h6> tags to the panel.

## buildCharts Function
The `buildCharts` function generates visualizations (Bubble Chart and Bar Chart) based on sample data retrieved from an external JSON file. It uses D3.js to fetch the data asynchronously. The function follows these steps:
- Asynchronously fetches data from an external JSON file using D3.js.
- Extracts the 'samples' array from the fetched data.
- Filters the 'samples' array based on the provided 'sample' ID.
- Extracts relevant data (OTU IDs, OTU labels, and sample values) to populate the charts.
- Builds a Bubble Chart displaying the distribution of bacteria cultures per sample.
- Builds a Bar Chart visualizing the top 10 bacteria cultures found in the sample.

## init Function
The `init` function initializes the webpage by populating a dropdown menu with sample names retrieved from an external JSON file. It then builds the initial plots based on the first sample from the dropdown. It follows these steps:
- Fetches data asynchronously from an external JSON file using D3.js.
- Extracts sample names from the fetched data.
- Populates the dropdown menu with sample names.
- Builds initial plots based on the first sample from the dropdown.

## optionChanged Function
The `optionChanged` function is triggered whenever a new sample is selected from the dropdown. It fetches new data and updates the plots and metadata accordingly.

References:
-In class activities
-ChatGPT to review the code
- youtube https://www.youtube.com/watch?v=ajdRvxDWH4w&list=PLGjplNEQ1it_oTvuLRNqXfz_v_0pq6unW
-BCS Support - Veerance for the initial code and Tumisang assisted in running of the dashboard in HTML.
