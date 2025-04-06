# Malaysia Bank List API

This repository hosts a list of Malaysian banks in a JSON format. The JSON file contains essential information about major banks in Malaysia, including their name, code, and SWIFT code. You can access and use this API to integrate the bank data into your applications.

## API Endpoint

The JSON file can be accessed at the following URL:

https://github.com/noobster97/malaysia-bank-list/banks.json


Simply use this link to retrieve the bank data in JSON format.

## Example Usage

### **JavaScript Example**

You can fetch the JSON data from this API using the `fetch()` function in JavaScript.

```javascript
fetch('https://github.com/noobster97/malaysia-bank-list/banks.json')
  .then(response => response.json())
  .then(data => {
    console.log(data);  // Logs the list of banks in the console
  })
  .catch(error => console.error('Error fetching bank data:', error));

Python Example
You can also use Python's requests module to fetch the JSON data.

import requests

url = "https://github.com/noobster97/malaysia-bank-list/banks.json"
response = requests.get(url)

if response.status_code == 200:
    banks_data = response.json()
    print(banks_data)  # Prints the list of banks
else:
    print("Failed to retrieve data.")

Using the Data
The JSON data includes the following fields for each bank:

name: Name of the bank

code: The bank's code

swift: The SWIFT/BIC code of the bank (if available)

Example JSON Structure

[
  {
    "name": "Maybank",
    "code": "MAYBANK",
    "swift": "MBBEMYKL"
  },
  {
    "name": "CIMB Bank",
    "code": "CIMB",
    "swift": "CIBBMYKL"
  },
  {
    "name": "Public Bank",
    "code": "PUBLICBANK",
    "swift": "PBBEMYKL"
  }
]

Contributing
If you have additional banks or updates to the bank list, feel free to contribute by creating a pull request with your changes. Please ensure that the data format remains consistent with the current structure.
