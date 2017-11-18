# UnityCSVReader
CSV Reader for Unity(implemented using C#)

If you want stable module, use https://github.com/JoshClose/CsvHelper

This CSVReader is implemented in a single file.  You can put (and remove) this class easily.

## How to use

```
// using System.IO;
var result = CSVReader.ParseCSV(File.ReadAllText(@"/Users/furukazu/data.csv"));

foreach(var result in data){
    foreach(var col in line){
        // process the data
    }
}

// read from Resource
// in this case, you place the csv file at Assets/Resources/CSV/data.csv 
var res = CSVReader.ParseCSV((Resources.Load("CSV/data") as TextAsset).text);

```

## License
MIT
