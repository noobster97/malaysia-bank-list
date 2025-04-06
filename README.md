# Malaysia Bank List API

This repository provides a JSON API containing a list of major banks in Malaysia, including their names, codes, and SWIFT/BIC codes.

## Accessing the JSON API

The JSON data can be accessed via the following URL:

https://noobster97.github.io/malaysia-bank-list/banks.json

## Example JSON Response

### The JSON API will return data in the following format:

``[
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
``

## Example Usage

### Fetch Data in JavaScript

You can easily fetch the bank list in your web application using JavaScript's `fetch()` method:

```javascript
fetch('https://noobster97.github.io/malaysia-bank-list/banks.json')
  .then(response => response.json())
  .then(data => {
    console.log(data); // Use the list of banks here
  })
  .catch(error => console.error('Error fetching data:', error));
