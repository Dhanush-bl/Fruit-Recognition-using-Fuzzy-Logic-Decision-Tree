# Fruit-Recognition-using-Fuzzy-Logic-Decision-Tree
<ul>
 <li>Fuzzy Decision trees can be used for identifying the fruits.<br>
<br><li>The FruitClassification.py is used to extract the fruit features based on which the classification of fruits can be done by constructing the decision tree for the features that we have extracted.<br>
<br><li>The features that we are considering is the<b> Mean of Red , Green and Blue value and geometric features such as Area, Perimiter and the shape of the fruit i.e Roundness.</b><br>
<br><li>Before we start with the feature extraction we need to do some preprocessing <b>i.e Finding the Contours for the image </b>for that we need to convert the image to gray scale and apply thresholding function using opencv(cv2).Then we draw the rectangle arround the largest contour that we have identified. <br>
 <br><li>Once we find the contours using <b>cv2.findcontour</b> then we identify the largest contour present in the image.<br>
<br><li>The Mean R,G and B value can be extracted by the following code :-
  
   &emsp;&emsp;<b>vg_color_per_row = np.average(img, axis=0)<br>
    &emsp;&emsp;avg_color = np.average(avg_color_per_row, axis=0)<br>
      &emsp;&emsp;[B,G,R]=avg_color<br><b></ul>
