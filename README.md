# Twitter Profile Scraper (Banao Task 2)

This project scrapes Twitter profile information (Bio, Followers, Following, Location, and Website) from a list of Twitter profile links using Selenium and BeautifulSoup.

## Directory Structure
```
vedantkale106-banao-task-2.git/
├── twitter_links.csv
├── twitter_profiles_scraped.csv
└── twitter_scraping.py
```

## Requirements
Ensure you have the following installed:
- Python 3.13.2
- Microsoft Edge browser
- Edge WebDriver

## Installation
Run the following command to install the required dependencies:
```bash
pip install pandas selenium beautifulsoup4 webdriver-manager
```

## Usage
1. **Prepare Input File:**
   - Add Twitter profile links in `twitter_links.csv` under the "Links" column.

2. **Run the Scraper:**
   ```bash
   python twitter_scraping.py
   ```

3. **Output File:**
   - Scraped profile data will be saved in `twitter_profiles_scraped.csv`.

## Output Format
The scraped data is stored in CSV format with the following columns:
```
Bio, Following Count, Followers Count, Location, Website, Profile_Link
```

## Notes
- This script automates logging into Twitter, so you must provide valid credentials inside `twitter_scraping.py`.
- If Twitter updates its UI or restricts automated access, the script might need adjustments.

## Troubleshooting
- If scraping fails due to login issues, verify your credentials.
- Ensure Edge WebDriver is installed and matches your browser version.
- If Twitter blocks your login attempts, consider adding delays or using a different IP.

## Disclaimer
This script is for educational purposes only. Scraping Twitter without permission may violate its terms of service. Use responsibly.
