# WebCrawling through Google CSE

# Google API Client and Beautifulsoup, urllib libraries are required 
'''
pip install --upgrade google-api-python-client 
pip install beautifulsoup, urllib
'''

# Caution

(1) Google CSE provides '10 Result * 10 Pages' and 100 query per day
    You cannot get more than 10 pages per query even if you pay for it.

(2) Google CSE is officially providing various search options but the result is different from Goodle Search.
    From my personal experience, one-site per one cse-id was the best. (2017.06)

(3) If you do google by using urllib, google will block the IP and asking 'are you robot'.

# Example
1. Setup the CSE Code and API

'''python
# You have to take a key from google CSE
# You can get an API key from https://developers.google.com/maps/documentation/javascript/get-api-key?hl=ko#key
my_api_key = "** YOUR API KEY **"

# You can setup the CSE and get CSE_ID from https://cse.google.com/cse/all
# You can add searching site in GUI interface 
# but it seems like *only one site per key is working properly* at the moment (17.06.05)
my_cse_id= "** YOUR CSE ID **"

# Insert the site in the CSE setup
search_site = "** SITE in the CSE setup **"
'''

2. Do the Search Query as below:

'''python
doSearchWithSaving("Search Term")
'''
