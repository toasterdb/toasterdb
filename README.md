# toasterdb
toasterdb is toy rust toy database

## concepts

**Write Amplification** 

Write amplification is the ratio of the amount of data written to the storage device versus the amount of data written to the database.
For example, if you are writing 10 MB to the database and you observe 30 MB disk write rate, your write amplification is 3.

**Read amplification**
Read amplification is the number of disk reads per query.

For example, if you need to read 5 pages to answer a query, read amplification is 5.

Note that the units of write amplification and read amplification are different. Write amplification measures how much more data is written than the application thought it was writing, whereas read amplification counts the number of disk reads to perform a query.

**Space amplification**
Space amplification is the ratio of the amount of data on the storage device versus the amount of data in the database.

For example, if you put 10MB in the database and this database uses 100MB on the disk, then the space amplification is 10.
