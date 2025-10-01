Recently **CEMS Early Warning Data Store** in their 31 Jan 2024's update,
announced that __*'Please note that accessing this dataset via CDS for time-critical operation is not advised or supported'*__ .
So, the previous system advised in CDS website (https://ewds.climate.copernicus.eu/how-to-api) is not working anymore.
User needs to change the api url to download the datasets as the new datasets are stored in https://ewds.climate.copernicus.eu/datasets.
So, this code provided here as CodeforGloFas.ipnyb will provide an easier way to download the same datasets from CEMS Early Warning Data Store (EWDS).
Things user need to think before using this:

Variable name → in EWDS, the variable is usually "dis24", not "river_discharge_in_the_last_24_hours" (that was CDS).

- How to get the correct token
  - Go to EWDS dashboard and log in (https://ewds.climate.copernicus.eu/profile).
  - In the top right, click on your username → Profile → API Key / Personal Access Tokens.
  - Copy the long UUID-style token (looks like what you pasted earlier, but it must be created in EWDS, not CDS).

- Variable name
  * You can confirm this on the dataset download page: click “Show API request” (example: https://ewds.climate.copernicus.eu/datasets/efas-forecast?tab=download)
