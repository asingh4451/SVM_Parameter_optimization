# SVM_Parameter_optimization
_Optimization of various parameters of SVM such as Gamma, Epsilon, Kernal,etc. to maximize the Accuracy_
# Datsaset
_Dataset used in this Parameter optimization is an Letter Recognition Dataset available on UCI Repository_
>Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.
  
  [Letter Recognition Data Set](https://archive.ics.uci.edu/ml/datasets/Letter+Recognition)
  # Overview Of Dataset
  |lettr|x-box|y-box|width|high|onpix|x-bar|y-bar|x2ba|y2bar|xybar|x2ybr|xy2br|x-ege|xegvy|y-ege|yegvx|
|-----|-----|-----|-----|----|-----|-----|-----|----|-----|-----|-----|-----|-----|-----|-----|-----|
|T    |2    |8    |3    |5   |1    |8    |13   |0   |6    |6    |10   |8    |0    |8    |0    |8    |
|I    |5    |12   |3    |7   |2    |10   |5    |5   |4    |13   |3    |9    |2    |8    |4    |10   |
|D    |4    |11   |6    |8   |6    |10   |6    |2   |6    |10   |3    |7    |3    |7    |3    |9    |
|N    |7    |11   |6    |6   |3    |5    |9    |4   |6    |4    |4    |10   |6    |10   |2    |8    |
|G    |2    |1    |3    |1   |1    |8    |6    |6   |6    |6    |5    |9    |1    |7    |5    |10   |
|S    |4    |11   |5    |8   |3    |8    |8    |6   |9    |5    |6    |6    |0    |8    |9    |7    |
|B    |4    |2    |5    |4   |4    |8    |7    |6   |6    |7    |6    |6    |2    |8    |7    |10   |
|A    |1    |1    |3    |2   |1    |8    |2    |2   |2    |8    |2    |8    |1    |6    |2    |7    |
|J    |2    |2    |4    |4   |2    |10   |6    |2   |6    |12   |4    |8    |1    |6    |1    |7    |
|M    |11   |15   |13   |9   |7    |13   |2    |6   |2    |12   |1    |9    |8    |1    |1    |8    |
|X    |3    |9    |5    |7   |4    |8    |7    |3   |8    |5    |6    |8    |2    |8    |6    |7    |
|O    |6    |13   |4    |7   |4    |6    |7    |6   |3    |10   |7    |9    |5    |9    |5    |8    |
|G    |4    |9    |6    |7   |6    |7    |8    |6   |2    |6    |5    |11   |4    |8    |7    |8    |
  
  **where**
  -  lettr	capital letter	(26 values from A to Z) **Output Value**
	 -  x-box	horizontal position of box	(integer)
	 -  y-box	vertical position of box	(integer)
	 -  width	width of box			(integer)
	 -  high 	height of box			(integer)
	 -  onpix	total # on pixels		(integer)
	 -  x-bar	mean x of on pixels in box	(integer)
	 -  y-bar	mean y of on pixels in box	(integer)
	 -  x2bar	mean x variance			(integer)
	 -  y2bar	mean y variance			(integer)
	 -  xybar	mean x y correlation		(integer)
	 -  x2ybr	mean of x * x * y		(integer)
	 -   xy2br	mean of x * y * y		(integer)
	 - x-ege	mean edge count left to right	(integer)
	 - xegvy	correlation of x-ege with y	(integer)
	 - y-ege	mean edge count bottom to top	(integer)
	 - 	yegvx	correlation of y-ege with x	(integer)
  
  # Data Output Table
|Sample|Best Accuracy     |Best Kernel|Best Nu|Best Epsilon|
|------|------------------|-----------|-------|------------|
|1     | 0.78             |linear     |1.21   |6.92        |
|2     | 0.78             | linear    | 1.21  | 6.92       |
|3     | 0.86             | rbf       | 8.19  | 0.71       |
|4     | 0.88             | rbf       | 2.08  | 2.05       |
|5     | 0.88             | rbf       | 2.08  | 2.05       |
|6     | 0.88             | rbf       | 2.08  | 2.05       |
|7     | 0.88             | rbf       | 2.08  | 2.05       |
|8     | 0.88             | rbf       | 2.08  | 2.05       |
|9     | 0.88             | rbf       | 2.08  | 2.05       |
|10    |0.95              | poly      | 9.61  | 2.96       |
  
  # Output Graph of Iterations and Best Accuracy
 ![output](https://user-images.githubusercontent.com/108614474/233383929-284cf141-e560-4a42-a8f3-0db92194845f.png)

