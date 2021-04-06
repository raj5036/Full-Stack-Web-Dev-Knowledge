# Full-Stack-Web-Dev-Knowledge

## Importing Data into a MongoDB Collection from a .csv/.xlsx files

1. Turn on the MongoDB server in your localmachine.
2. Fire up a terminal and head over to the directory where the file is stored.
3. Now run the following command 

```
mongoimport --type csv -d test -c products --headerline --drop products.csv
```

>We’ll explain the flags we used but you can also use the help command mongoimport --help to get the same information.
>
> –type: The input format to import: json, csv, or tsv. We are using csv so that’s what we specify.\
> -d: Specifies what database to use. We used the test database.\
> -c: Specifies what collection to use. We used a collection called products.\
> –headerline: Specifies that the first row in our csv file should be the field names.\
> –drop: Specifies that we want to drop the collection before importing documents.\
