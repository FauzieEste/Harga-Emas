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

const Start = async () => {
  try {
    const data = await hargaemas();
    console.log(data);
  } catch (error) {
    console.error("Error occurred:", error.message);
  }
};

Start();

```
## Example Output
```javascript
Data Emas: {
  DevInfo: {
    Developer: 'Fauzie Este',
    Tools: 'Harga Emas Scraper',
    Information: 'Data Diambil dari : https://harga-emas.org/1-gram/'
  },
  DataEmas: {
    USDData: { USD: '69,32 ↑ ', Persentase1: '+0,29', Persentase2: '+0,42%' },
    IDRData: {
      IDR: '1.084.479,03 ↑ ',
      Persentase1: '+4.090,56',
      Persentase2: '+0,38%'
    },
    KURSData: {
      KURS: '15.644,70 ↓ ',
      Persentase1: '-7,05',
      Persentase2: '-0,05%'
    }
  }
}
```
## License

[MIT](https://choosealicense.com/licenses/mit/)

Last Update on : 07 March 2024 by FauzieEste.