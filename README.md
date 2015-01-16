# pyspark-pictures
Learn the pySpark API though pictures and simple examples

![example image](./images/readme-example.png)

```python
# flatMap
x = sc.parallelize([1,2,3])
y = x.flatMap(lambda x: (x, 100*x, x**2))
print(x.collect())
print(y.collect())
```
[1, 2, 3]
[1, 100, 1, 2, 200, 4, 3, 300, 9]

## [View Static Version](http://nbviewer.ipython.org/github/jkthompson/pyspark-pictures/blob/master/pySpark-pictures.ipynb)

## Install Interactive Version
1. install [Spark](https://spark.apache.org/)
2. install [IPython notebook](http://ipython.org/notebook.html)
3. start pySpark inside IPython notebook

```
IPYTHON_OPTS="notebook --pylab inline" pyspark
```

4) open pySpark-pictures.ipynb 

