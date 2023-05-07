# manuscript-central-checker
A Python-based script to check the status of transactions and journals on Manuscript Central

The script has been tested on Python 3.6 with ChromeDriver 98.0.4758.102

Requirements:
- Python >=3.6
- Selenium (`pip install selenium`)
- ChromeDriver (https://chromedriver.chromium.org/downloads)

After installing the required packages, place the ChromeDriver in the same folder of the script and run the script as follows:

`python msc_script.py -j websites.json -t timeout`

where:
- -j JSON, --json JSON: a json file containing the list of websites to check along with username, password, and the number of max entries to report [optional] (a template json file is provided)
- -t TIMEOUT, --timeout TIMEOUT: [optional] timeout waiting for website response (default=2)


This tool has been tested on:
- ACM Computing Surveys (https://mc.manuscriptcentral.com/csur)
- ACM Distributed Ledger Technologies (https://mc.manuscriptcentral.com/dlt)
- ACM Transactions on Intelligent Systems and Technology (https://mc.manuscriptcentral.com/tist)
- IEEE Communications Surveys and Tutorials (https://mc.manuscriptcentral.com/comst-ieee)
- IEEE Journal of Biomedical and Health Informatics (JBHI) (https://mc.manuscriptcentral.com/jbhi-embs)
- IEEE Transactions on Computers (TC) (https://mc.manuscriptcentral.com/tc-cs)
- IEEE Transactions on Emerging Topics in Computing (TETC) (https://mc.manuscriptcentral.com/tetc-cs)
- IEEE Transactions on Information Forensics and Security (TIFS) (https://mc.manuscriptcentral.com/sps-ieee)
- IEEE Transactions on Parallel and Distributed Systems (TPDS) (https://mc.manuscriptcentral.com/tpds-cs)
- IEEE Transactions on Very Large Scale Integration (TVLSI) (https://mc.manuscriptcentral.com/tvlsi-ieee) (JSON key should be Transactions on Information Forensics)
- IEEE Transactions on Systems, Man and Cybernetics: Systems (SMC: Systems) (https://mc.manuscriptcentral.com/systems)