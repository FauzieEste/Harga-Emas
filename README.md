# Harga Emas / Gold Price Scraper

Data fetch from : https://harga-emas.org/1-gram/

## Installation

Use the package manager [npm](https://docs.npmjs.com/cli/v8/commands/npm-install) to install module.

```bash
npm i harga-emas-scraper
```

## Example Usage

```javascript
const hargaemas = require('harga-emas-scraper');

async function Start() {
  try {
    const data = await hargaemas();
    console.log(data);
  } catch (error) {
    console.error("Error occurred:", error.message);
  }
}

Start();

```
## Example Output
```javascript
{
  "DevInfo": {
    "Developer": "Fauzie Este",
    "Tools": "Harga Emas Scraper",
    "Information": "Data Diambil dari : https://harga-emas.org/1-gram/"
  },
  "DataEmas": {
    "IDRData": {
      "IDR": "1.084.742,57 ↑ ",
      "Persentase1": "+4.354,10",
      "Persentase2": "+0,40%"
    },
    "USDData": {
      "USD": "69,26 ↑ ",
      "Persentase1": "+0,23",
      "Persentase2": "+0,33%"
    },
    "KURSData": {
      "KURS": "15.660,85 ↑ ",
      "Persentase1": "+9,10",
      "Persentase2": "+0,06%"
    }
  }
}
```
## License

[MIT](https://choosealicense.com/licenses/mit/)

Last Update on : 07 March 2024 by FauzieEste.