# Full-Stack-Web-Dev-Knowledge

## Importing Data into a MongoDB Collection from a .csv/.xlsx files

1. Turn on the MongoDB server in your localmachine.
2. Fire up a terminal and head over to the directory where the file is stored.
3. Now run the following command 

```
mongoimport --type csv -d test -c products --headerline --drop products.csv
```
