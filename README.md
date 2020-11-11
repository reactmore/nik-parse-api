# USAGE

```
//Console log
var nik = require("./index");

console.log(nik.nikParse(3271012707960007))
```
```
//express js

app.get('/api/nik/:nik', function (req, res) {
    const nik = req.params["nik"];
    res.send(induk.nikParse(nik));
  });
  
//ex : https://your-domain/api/nik/3271012079730007  
```

Result
```json
{
  "status": "success",
  "pesan": "NIK valid",
  "data": {
    "nik": "3204110609970001",
    "kelamin": "LAKI-LAKI",
    "lahir": "06/09/1997",
    "provinsi": "JAWA BARAT",
    "kotakab": "KAB. BANDUNG",
    "kecamatan": "KATAPANG",
    "uniqcode": "0001",
    "tambahan": {
      "kodepos": "40921",
      "pasaran": "Sabtu Pahing, 6 September 1997",
      "usia": "23 Tahun 1 Bulan 27 Hari",
      "ultah": "10 Bulan 8 Hari Lagi",
      "zodiak": "Virgo"
    }
  }
}
```

<h3>- <a href="https://github.com/bachors/nik_parse.js
">Original Repo</a></h3>
