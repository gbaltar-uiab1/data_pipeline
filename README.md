# data_pipeline
Construción dun Pipeline de Datos Multibase con Docker e Python

## Conxunto de dados

O conxunto de datos escolleito é `books.csv`, parte da colleita [*Books Dataset* de Kaggle](https://www.kaggle.com/datasets/saurabhbagchi/books-dataset).

## Como executar os servizos Docker

O arquivo `docker-compose.yml` ten que se atopar no cartafol de traballo (CWD).<br>
En Linux/WSL executamos con <br>
`sudo docker-compose up -d`

Podemos comproba-lo estado dos servizos co caderno Jupyter `service-test.ipynb`.


## Como reproducir os notebooks

Para executa-las operacións da tubaxe de dados (*data pipeline*) hai que escrebar cos servizos de Docker que as apoian (v. apartado anterior).

Unhas operacións dependen das outras, polo que cómpre executa-los cadernos de xeito secuencial.

`1.CargarMySQL.ipynb` > 
`2.CargarCassandra.ipynb` > 
`3.CargarRedis.ipynb` > 
`4.CargarMongoDB.ipynb`.

## Dete-los servizos de Docker logo de rematar.

Se xa non os precisamos, podemos detelos.
En Linux/WSL executamos a seguinte orde: <br>
`sudo docker-compose down`

Podemos comproba-lo estado dos servizos co caderno Jupyter `service-test.ipynb` ou coa orde `sudo docker ps`.

以上
