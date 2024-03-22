﻿# JUS-TCU

A web-scraping project created to capture data from [Brazillian Federal Court of Accounts](https://portal.tcu.gov.br/inicio/). It basically accesses a website, downloads every report in the range (user's decision) and using regex expression, captures the plenary session's decisions (called acórdãos) from pdf files and save it in an excel file. These reports are weekly posted and are very important to Federal Court of Account and others related.

## How can I run?

1. Clone this repository ```git clone https://github.com/joaocansi/jus-tcu.git```
2. Access the project folder ```cd jus-tcu```
3. Install project dependencies ```pip install openpyxl selenium docx2txt PyMuPDF webdriver-manager```
4. Run the project ```python src/main.py <from> <to>```

OBS: <from> and <to> are the range of reports. For example, if <from> equals 10 and <to> equals 20, the script will return the data from report of number 10 to report of number 20.
