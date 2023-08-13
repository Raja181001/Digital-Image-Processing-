from numpy import *
from matplotlib.pyplot import *
from PIL import Image
import cv2
from google.colab.patches import cv2_imshow
from google.colab import drive 
drive.mount('/content/drive')


          #Step 1 : Extracting the image and converting the image into grayscale 
img1 = cv2.imread('/content/drive/MyDrive/DIP/Grey_scale.png')
img = cv2.cvtColor(img1,cv2.COLOR_BGR2GRAY)
print('Original Image')
cv2_imshow(img)
print('\n')

          #Step 2 : Formaing empty matrix which will be furter converted to bit planes

b1 = matrix(zeros(img.shape))
b2 = matrix(zeros(img.shape))
b3 = matrix(zeros(img.shape))
b4 = matrix(zeros(img.shape))
b5 = matrix(zeros(img.shape))
b6 = matrix(zeros(img.shape))
b7 = matrix(zeros(img.shape))
b8 = matrix(zeros(img.shape))

        #Step 3 : Defining a function for conveting the numerics to binary 

def binary(x):
  if(x==0):
    return
  else:
    binary(int(x/2))
    r=x%2
    l.append(r)

print(img.shape)
for i in range(183):
  for j in range(275):
    l=[]
    


    binary(img[i,j])
    if img[i,j] == 1:
      b8[i,j] = l[0]
    elif 1<img[i,j]<4:
      b8[i,j] = l[1]
      b7[i,j] = l[0]
    elif 3<img[i,j]<8:
      b8[i,j] = l[2]
      b7[i,j] = l[1]
      b6[i,j] = l[0]
    elif 7<img[i,j]<16:
      b8[i,j] = l[3]
      b7[i,j] = l[2]
      b6[i,j] = l[1]
      b5[i,j] = l[0]
    elif 15<img[i,j]<32:
      b8[i,j] = l[4]
      b7[i,j] = l[3]
      b6[i,j] = l[2]
      b5[i,j] = l[1]
      b4[i,j] = l[0]
    elif 31<img[i,j]<64:
      b8[i,j] = l[5]
      b7[i,j] = l[4]
      b6[i,j] = l[3]
      b5[i,j] = l[2]
      b4[i,j] = l[1]
      b3[i,j] = l[0]
    elif 63<img[i,j]<128:
      b8[i,j] = l[6]
      b7[i,j] = l[5]
      b6[i,j] = l[4]
      b5[i,j] = l[3]
      b4[i,j] = l[2]
      b3[i,j] = l[1]
      b2[i,j] = l[0]
    elif 127<img[i,j]<256:
      b8[i,j] = l[7]
      b7[i,j] = l[6]
      b6[i,j] = l[5]
      b5[i,j] = l[4]
      b4[i,j] = l[3]
      b3[i,j] = l[2]
      b2[i,j] = l[1]
      b1[i,j] = l[0]

          #Getting different types of images with the help of the bit planes obtained 

print('image having most significant bit plane to zero')
h = pow(2,6)*b2 + pow(2,5)*b3 + pow(2,4)*b4 + pow(2,3)*b5 + pow(2,2)*b6 + pow(2,1)*b7 + pow(2,0)*b8
cv2_imshow(h)
print('\n')
print('image having least significant bit palne to zero')
h1 = pow(2,7)*b1 + pow(2,6)*b2 + pow(2,5)*b3 + pow(2,4)*b4 + pow(2,3)*b5 + pow(2,2)*b6 + pow(2,1)*b7
cv2_imshow(h1)
print('\n')
print('image of eighth bit plane')
h2 = pow(2,7)*b1
cv2_imshow(h2)
print('\n')
print('image of seventh bit plane')
h3 = pow(2,6)*b2
cv2_imshow(h3)
print('\n')
print('image of sixth bit plane')
h4 = pow(2,5)*b3
cv2_imshow(h4)
print('\n')
print('image of fifth bit plane')
h5 = pow(2,4)*b4
cv2_imshow(h5)
print('\n')
print('image of fourth bit plane')
h6 = pow(2,3)*b5
cv2_imshow(h6)
print('\n')
print('image of third bit plane')
h7 = pow(2,2)*b6
cv2_imshow(h7)
print('\n')
print('image of second bit plane')
h8 = pow(2,1)*b7
cv2_imshow(h8)
print('\n')
print('image of first bit plane')
h9 = pow(2,0)*b8
cv2_imshow(h9)
