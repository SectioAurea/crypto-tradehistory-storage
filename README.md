crypto-tradehistory-storage
===========================

Python code to store trade history from cryptocurrency broker APIs. Currently supports Cryptsy. Run via Cron.

Example crontab entry for 15 minutes frequency:

0,14,29,44 * * * * cd /home/tradehistory/crypto-tradehistory-storage && python cron.py


Dependencies: 

-- SQLite3 package ('sqlite3' on Ubuntu)
Make sure the directory for the database entries exists, by default this is db/ in the same directory.
The scraper code does not handle this directory's creation, it assumes it exists.

-- Cryptsy API library v0.2 (or better)
https://github.com/jaapz/CryptsyPythonAPI

Cryptsy.php should be in same directory as cron.py and scrape.py.

Please visit #cryptoforex in Freenode for support or questions.
