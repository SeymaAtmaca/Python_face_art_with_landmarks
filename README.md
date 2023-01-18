## Technologies
<ul>
<li> :snake: Python </li>
</ul>

<br>
<h1> :waning_crescent_moon: :star: Türkçe  </h1> 
Bu repo, landmark ile yüz tespiti gerçekleştiren, görüntü üzerinde en çok kullanılan renkleri tespit eden ve bu renkler aracılığı ile yüz üzerinde dairesel filtre uygulayan bir Python projesini içermektedir. <br><br>
Landmark ile tespit edilen yüz ve yüzdeki noktalar, Notebook' da görüldüğü gibi görüntü üzerinde çizdirilmektedir. Tespit edilen noktalar üzerinden yüz hattı noktaları ve iki göz arasında bulunan orta nokta bir array üzerinde kaydedilir. Daha sonra görüntü üzerinde en çok kullanılan 6 renk KMeans ile bulunur ve colors[] array' inde depolanır. <br><br>
Alınan renkler ile yüz noktaları üzerinde bir maske oluşturulur. Bu maske bölgesine uygulanmak üzere, en çok kullanılan 6 renk ile daireler çizdirilerek filtre görüntüsü oluşturulur. Bu çizdirme işlemi cv2.circle ile gerçekleştirilir. Daha sonra bu daireli görüntü maskeye uygulanır ve görüntüye aktarılacak ana bölüm eld edilir. <br><br>
Maske ve filtre elde edildikten sonra görüntü üzerine filtre uygulanır. BU uygulama işlemi cv2.bitwise_or ya da cv2.bitwise_xor ile gerçekleştirilir. <br><br><br>


<h1> English </h1>
This repo includes a Python project that performs face detection with landmark, detects the most used colors on the image, and applies circular filters on the face through these colors. <br><br>
The face and the points on the face detected with the Landmark are drawn on the image as seen in the Notebook. Over the detected points, the facial line points and the midpoint between the two eyes are recorded on an array. Then, the 6 most used colors on the image are found with KMeans and stored in the colors[] array. <br><br>
A mask is created on the face points with the imported colors. A filter image is created by drawing circles with the 6 most used colors to be applied to this mask region. This plotting is done with cv2.circle. Then this circular image is applied to the mask and the main part to be transferred to the image is obtained. <br><br>
After the mask and filter are obtained, the filter is applied on the image. This application process is performed with cv2.bitwise_or or cv2.bitwise_xor.
<br><br><br>

* <b> Türkçe : </b> Aşağıda örnek çıktılar yer almaktadır. 
* <b> English : </b> Below are examples.

<br>

![h.png](https://github.com/SeymaAtmaca/Python_face_art_with_landmarks/blob/main/images/h.jpg) <br><br>
![p.png](https://github.com/SeymaAtmaca/Python_face_art_with_landmarks/blob/main/images/p.png)<br><br>

<br> 
<b> Outputs : </b><br><br>

![j.png](https://github.com/SeymaAtmaca/Python_face_art_with_landmarks/blob/main/images/j.png) ![o.png](https://github.com/SeymaAtmaca/Python_face_art_with_landmarks/blob/main/images/o.png)

<br><br>



## Contact

 My [LinkedIn](https://www.linkedin.com/in/%C5%9Feyma-atmaca-925b57195/) profile.
