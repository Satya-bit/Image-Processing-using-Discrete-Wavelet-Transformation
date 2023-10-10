# Image-Processing-using-Discrete-Wavelet-Transformation
**=>Objective**

Three type of image is processing can be done:

●Image Restoration : Resultant image will be a restored image of more than one degraded
images.

●Image Mixing : More than two images can be fused to form a new image that will contain
information of every input image.

●Image Morphing : Image morphing is done to achieve face morphing from faces of two different
persons.

**=>Techniques**

* Firstly, the user has to select images that he wants for image
processing as an input.

* Single Level Wavelet Decomposition is used. Once we get those images, I decomposed both the images separately into
the wavelet coefficients using discrete Wavelet Transform.

*After the decomposition of Images I got 4 matrices of coefficients where
each matrice will depict:

->Approximate coefficient of Image

->Horizontal Detailed coefficient of Image

->Vertical Detailed coefficient of Image

->Diagonal Detailed coefficient of Image

* So after decomposition of Images is done, I fused all these wavelet coefficient
matrices to achieve the fused decomposition matrices.

* Lastly when I got the Fused decomposition Matrix I did inverse
Discrete Wavelet Transform for the final output of the process.

![image](https://github.com/Satya-bit/Image-Processing-using-Discrete-Wavelet-Transformation/assets/70309925/87db2004-7d00-446e-9947-87f6185454c2)


**=>Process**

* In our project we will be doing sub band fusion of the decomposition image that we got
earlier for the fusion process.

cA = fusion1(cA1, cA2)

cH = fusion2(cH1, cH2)

cV = fusion2(cV1, cV2)

cD = fusion2(cD1,cD2)

* The fusion1 and fusion2 are the mathematical operation for fusion

Fusion1 : for Approximation Coefficient

Fusion2 : for Detailed Coefficient

* Fusion1 and Fusion2 can be Mean, Max and Min mathematical operation.

For example in above equation we wrote,

cA = fusion1(cA1, cA2) = mean(cA1,cA2).

![image](https://github.com/Satya-bit/Image-Processing-using-Discrete-Wavelet-Transformation/assets/70309925/a45714d6-3ca9-448d-bb58-698afb6501a4)

![image](https://github.com/Satya-bit/Image-Processing-using-Discrete-Wavelet-Transformation/assets/70309925/fbd0809c-a25a-47ec-880a-c4486c7c8e9d)

![image](https://github.com/Satya-bit/Image-Processing-using-Discrete-Wavelet-Transformation/assets/70309925/5bc23a85-2400-420b-821d-607e10f2ea7b)

![image](https://github.com/Satya-bit/Image-Processing-using-Discrete-Wavelet-Transformation/assets/70309925/f46b3390-1753-4bae-a983-8d69eeffcaa6)
