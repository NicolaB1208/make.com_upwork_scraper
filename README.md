# make.com Upwork Scraper #
A web scraper specifically for Upwork 'find_job' results. It scrapes the relevant information for each job and saves it to a Google Sheet.

<img width="1648" alt="Screenshot 2024-10-16 at 22 01 47" src="https://github.com/user-attachments/assets/331300dc-a1b1-4f40-b9bb-5f634123d05b">

### Goal of this automation ###
Have a straightforward way to get all the interesting job postings, go through them quickly, and note the ones worth checking in more detail.

## How it works ##

* Takes as input the link of the results page of a search:
  
<img width="1374" alt="Screenshot 2024-10-16 at 22 03 54" src="https://github.com/user-attachments/assets/9ca2fdc6-1fd3-492c-baa5-f2b7e1809794">

* Parses HTML to text.
* Extracts the JobID of each job.
* Recreates the URL of each job.
* Checks Google Sheet to see if the job URL is already there.
* For the new ones, makes a request to each individual job URL.
* Uses a series of regex patterns to extract all the relevant information.
* Pastes all the information into the Google Sheet.

<img width="1733" alt="Screenshot 2024-10-16 at 22 11 28" src="https://github.com/user-attachments/assets/d738bf5a-db7b-405b-abea-17d90c49c259">

### How to use it: ###

Download the `makeBlueprint_upwork_Webscraper_toSheets.json` file and import it as a blueprint in a new scenario in make.com.

<img width="789" alt="Screenshot 2024-10-16 at 22 16 30" src="https://github.com/user-attachments/assets/1c798a50-1e15-4bd4-9246-5fa018f29b0d">

