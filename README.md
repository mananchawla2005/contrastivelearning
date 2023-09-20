# Contrastive Learning using Point Cloud

- Colab Link [Click Here](https://colab.research.google.com/drive/1NVKW1RwpcvhRGVehLLNC5BpU8HINO5YV?usp=sharing)
- Dataset Used: SHAPENET 
# Model
This repository explores the task of contrastive learning applied to 3d point clouds using SimCLR model.
- <b>SimCLR MODEL:</b>
  <br>
  ![simclr-general-architecture](https://github.com/mananchawla2005/contrastivelearning/assets/42414965/fb63c442-55f9-4594-a5e0-98d6ab889721)
- <b>NTXENT Loss:</b>
  ![image](https://github.com/mananchawla2005/contrastivelearning/assets/42414965/4588825e-379e-4236-aad3-ebcd9a51e1f7)
The above image is the mathematical formula for NTXENT Loss introduced by SimCLR model. The numerator comprises of taking consine similarity of the the positive pairs which would lie between -1 to 1. It is then divided by a constant T or temperature and exponential of the value is taken to make it positive. The denominator comprises of summision of exponential of cosine similarity of negative pairs from 0 to 2N ( 2N for augmented pairs ). We dont sum the denominator for k=i ( i.e same as numerator ). Logarithm of whole thing is taken to soften the loss followed by a negative sign.

# Results
![image](https://github.com/mananchawla2005/contrastivelearning/assets/42414965/186ee5e5-e301-42ce-aa00-4ffe6971d82b)
![image](https://github.com/mananchawla2005/contrastivelearning/assets/42414965/e64bf51b-0deb-464e-990d-7ef82aaaa1d3)
![image](https://github.com/mananchawla2005/contrastivelearning/assets/42414965/266aa9c6-f453-43ce-86b5-871bdbb3dbb9)
![image](https://github.com/mananchawla2005/contrastivelearning/assets/42414965/835a7e0f-ffd9-4b66-8145-ce6fb18f7f0a)




