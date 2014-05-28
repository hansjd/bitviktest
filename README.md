#CCA2
CCA2 is a very simple


###Installation
	npm install cca2
	

### Usage
add CCA2 to your js file.

	var cca2 = require("CCA2");

---
convert country name to Country Code Alpha 2.

	var countryName = "faroe islands";
	var countryCode = cca2.getCode(countryName);
	console.log( "Country code for '" + countryName + "' is [" + countryCode + "].");

will output.

	"Country code for 'faroe islands' is [FO]."

---
convert Country Code Alpha 2 to country name .

	var countryCode = "fo";
	var countryName = cca2.getName(countryCode);
	console.log( "Country name for [" + countryCode + "] is '" + countryName + "'.");

will output.

	"Country name for [fo] is 'FAROE ISLANDS'."

*notice*<br>
although input is cas insensitive, output is always returned in UPPERCASE.

###countries.json
countries.json contains all the country name and country code in a json format<br>
template.
```json
{
	"AF": [
		"AFGHANISTAN"
	],
	"VG": [ // Country code (unique)
		"BRITISH VIRGIN ISLANDS", // Primary country
		"VIRGIN ISLANDS, BRITISH"
	],
	"DISCARDET": [ //"Countries" without country code
		"AKROTIRI",
		"ARCTIC OCEAN"
	]
}
```
