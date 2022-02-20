# MongoNessus
Automate the export and import of Nessus scan info into MongoDB. You'll need a working [Nessus Vulnerability Scanner](https://www.tenable.com/) and [MongoDB](https://www.mongodb.com/) instance.


## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pandas and pymongo.

```bash
pip install pymongo
pip install pandas
```

Create secrets.py and include the following.
```python
# secrets.py
secrets = {
    'NESSUS_URL': "",
    'NESSUS_ACCESS_KEY': "",
    'NESSUS_SECRET_KEY': "",
    'MONGO_URL': ""
}
```
Add the following to .gitignore
```
*.csv
secrets.py
__pycache__/
```
## Usage

```bash
python3 nessus.py
```
