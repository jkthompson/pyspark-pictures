# pyspark-pictures
Learn the pyspark API through pictures and simple examples

## Example:
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

## [View static version on NBViewer](http://nbviewer.ipython.org/github/jkthompson/pyspark-pictures/blob/master/pyspark-pictures.ipynb)

## Install (for interactive use)
1. install [Spark](https://spark.apache.org/)
2. install [IPython notebook](http://ipython.org/notebook.html)

## Quick Start
1. start pyspark inside IPython notebook
 	
	```bash
	IPYTHON_OPTS="notebook" pyspark
	```

2. open browser to notebook link 
3. open pyspark-pictures.ipynb 
4. edit example code, press: <kbd>ctrl</kbd> + <kbd>enter</kbd> to run each cell 

## References
[pyspark API](http://spark.apache.org/docs/1.2.0/api/python/index.html)

## Contribute
Contributors are welcome  
Original images are [here](https://docs.google.com/presentation/d/1VFX9WMHcYiDidWdY_uYbBIFqYjG6joxN817Y6l-jD5w/edit?usp=sharing), download to pdf, convert to svg with: genSVD (pdf2svg)
