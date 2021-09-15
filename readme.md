# Autolab Flask test
Autolab Pokemon


## Instructions

First install all of the Python requirements (via pip):

```sh
$ pip install -r requirements.txt
```

Before running the application, we need to run the database files to setup the database, tables and data.
To create the database, run the following command:
```sh
$ python data/data-db.py
```

Lastly, for running the application, use the command below:
```sh
$ python app.py
```

## Directories

- api : Have the endpoints definition code
    There are two endpoints, which have the following structure:

| Name |  |Url |
| ------ | ---|------ |
| pokemons |Retrieves all data from the DB |[http://127.0.0.1:5000/api/pokemons][PlDb] |
| pokemon | Can receive parameters for retrieve data filtered by ID  |[http://127.0.0.1:5000/api/pokemon?filter=1][PlGh] |
| pokemon | Can receive parameters for get response, sorted by indicated column and  ASC (by default) or DESC criteria |[http://127.0.0esting
.1:5000/api/pokemon?sort_ord=asc&sort_col=id][PlGh] |
| pokemon | In addition api was built for receive the combination for sorting and filtering |[http://127.0.0.1:5000/api/pokemon?sort_ord=asc&sort_col=id&filter=1][PlGh] |

## Test
Test were built using pytest, they could be run with the script:
```sh
$ pytest
```
![](https://github.com/rsh456/autolab/blob/main/pytest.jpg)

