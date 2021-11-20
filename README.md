# Victorian_Covid_Exposure_Sites_Checker


## **Archived due to the halting of contact tracing from now onwards.**

### What
- A little tool I built to check if you have been to any of the 100 most recent\* tier 1\** Victorian COVID-19 exposure sites
- \* The API is currently only returning the 100 most recent - working on it
- \** The API has changed to only show tier 1 sites because it is becoming too hard to track with so many cases.

### How To Use It
1. Enter the names of suburbs you have visited into `locations.json`
	- `Public Transport` considered its own suburb
		<details>
			<summary>Example</summary>
	
			{
				"locations": [
					"Melbourne",
					"Public Transport"
				]
			}
	
		</details>
2. Run `victorian_covid_exposure_site_checker.py` using a python 3 client

### How It Works
- Gets data from the DHHS Exposure site CKAN Data API, and checks for matches on locations.json

