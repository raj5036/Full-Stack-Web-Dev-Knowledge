# Full-Stack-Web-Dev-Knowledge

# Table of contents
1. [Git](#Git)
2. [MongoDB](#)
   * [Import data from csv files](#csv)
   * [Delete all data from a collection](#delCollection)
3. [JavaScript Essentials](#javascript-essentials)
   * [Execution Context](#execution-context)
   * [Callbacks in JavaScript](#)
   * [Hoisting](#)
   * [async-await](#)
   * [Closures](#)
 

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

## JavaScript Essesntials <a href="#javascript-essentials"></a>

### Execution Context <a href="#execution-context"></a>

  In JavaScript, execution context is an abstract concept that holds information about the environment within which the current code is being executed.
  
  Remember: the JavaScript engine creates the global execution context before it starts to execute any code. From that point on, a new execution context gets created every time   a function is executed, as the engine parses through your code. In fact, the global execution context is nothing special. It’s just like any other execution context, except     that it gets created by default.
