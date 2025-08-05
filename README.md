# 🐦 Twitter Data Scraping with Colab
This repository provides step-by-step notebooks to extract tweets using an active Twitter session and browser developer tools. It is built for users who want to scrape tweets without using the Twitter API, especially helpful after API access restrictions.
# 📁 Repository Structure
| File / Notebook                 | Description                                                         |
| ------------------------------- | ------------------------------------------------------------------- |
| `data.txt`                      | Required input: paste your session data here from browser dev tools |
| `Convert_txt_to_json.ipynb`     | Converts `data.txt` into usable `data.json` for request headers     |
| `Tweets_With_Keywords.ipynb`    | Extracts tweets based on your keywords and date range               |
| `Tweets_Without_Keywords.ipynb` | Extracts tweets from a user timeline without filtering by keyword   |
| `Combine_Excel_files.ipynb`     | Combines multiple Excel output files into a single dataset          |
| `README.md`                     | Guide and documentation                                             |
# 🚀 Requirements
Google Colab (you don’t need local setup)

A browser (Chrome/Firefox) and your active Twitter account

Ability to inspect network requests via DevTools (F12)

# 📌 Instructions
✅ First:
Log into your Twitter account.

Open Developer Tools in your browser (F12), go to the Network tab.

Copy the request headers from a tweet-related request.

Paste the entire headers into data.txt.

Run Convert_txt_to_json.ipynb to create data.json.

✅ Second:
Open Tweets_With_Keywords.ipynb.

Set your keywords and date range.

Run the notebook on Colab.

✅ Third (optional):
If you don’t want keyword filtering, use Tweets_Without_Keywords.ipynb.

After collecting data, run Combine_Excel_files.ipynb to merge outputs.
# 👩‍💻 Author
Mona Faghfouri Azar
Data Analyst | NLP Researcher
GitHub: @MonaFaghfouri

