# TrafficAccidentAnalysis
This project focuses on analyzing traffic accidents that have occurred and been recorded in Porto Alegre over the past four years. The goal is to gain insights into the patterns, causes, and trends of these accidents in order to improve road safety measures.

## Project Overview and Functionality
The Main file performs the following functions:

- Connects to the endpoint of the open data from Porto Alegre.
- Connects to AWS S3.
- Creates a session in PySpark, a dataframe, and connects it to the endpoint data.
- Performs data cleaning.

The Tests file:

- Connects to the sharpfile.
- Reads it into a Pandas dataframe.
- Executes column comparisons to enable proper address cleaning for joining with the traffic accident table.
- Performs some preliminary analysis and tests to enhance understanding of the dataset.

## Prerequisites
Before running the program, make sure to set the environment variables with the values of your AWS S3 account. If you don't want to save the database in AWS, you will need to comment out the relevant code sections in the main function (fifth cell).

Please note that this project was created using Anaconda dependencies, so it may not work in environments outside of Anaconda.

## Installation
To install the required dependencies, run the following command at the root of the project, where the requirements.txt file is located:

```pip install -r requirements.txt```

## Usage
- Load the Jupyter Notebook.
- Execute the main function.
- After running the main function, you can execute the tests to verify the correctness of the analysis.

## Output
The script generates a CSV file after execution, which can be further analyzed using various data visualization tools.

## Data Reliability
The data used in this project is provided by https://dadosabertos.poa.br. The reliability of the data is the responsibility of the source. You can explore other endpoints available on their website.
The data cleaning and analysis performed in this project correspond to the data provided until May 29th. It may be necessary to execute additional functions to extract more up-to-date data in the future.

## Future Work
- Improve the response time of the map in Tableau

To check and interact with the map, please access (please let me know if the website is down):
https://public.tableau.com/app/profile/murillo.masson/viz/TrafficAccidentPoAMap/histria?publish=yes

Feel free to explore the code and customize it according to your needs. Happy analyzing!

## Tableau's view
<div class='tableauPlaceholder' id='viz1685554264092' style='position: relative'><noscript><a href='#'><img alt='acidentes de trânsito ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Tr&#47;TrafficAccidentPoAMap&#47;histria&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='TrafficAccidentPoAMap&#47;histria' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Tr&#47;TrafficAccidentPoAMap&#47;histria&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='pt-BR' /><param name='filter' value='publish=yes' /></object></div>

<div class='tableauPlaceholder' id='viz1685554301694' style='position: relative'><noscript><a href='#'><img alt='acidentes de trânsito ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;YX&#47;YXZ76MXZP&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='path' value='shared&#47;YXZ76MXZP' /> <param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;YX&#47;YXZ76MXZP&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='pt-BR' /><param name='filter' value='publish=yes' /></object></div>                
