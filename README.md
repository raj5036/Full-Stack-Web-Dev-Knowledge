# Full-Stack-Web-Dev-Knowledge

# Table of contents
1. [Git](#Git)
2. [MongoDB](#)
   * [Import data from csv files](#csv)
   * [Delete all data from a collection](#delCollection)
 

## Undo Git init <a name="Git"></a>

1.Fire up the terminal.\
2.Get inside that intended directory.\
3.And run the following command.

```
rm -rf .git
```

## Importing Data into a MongoDB Collection from a .csv/.xlsx files <a name="#csv"></a>

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
> –drop: Specifies that we want to drop the collection before importing documents.

For detailed overview [Click here!](https://kb.objectrocket.com/mongo-db/how-to-import-a-csv-into-mongodb-327)


## MongoDB CLI commands

### Delete all from collections <a name="#delCollection"></a

```
db.user.remove({})
```
