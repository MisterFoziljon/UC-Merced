## Tensorflow datasets: uc_merced dataseti

#### 1. ```uc_merced``` dataseti haqida qisqacha ma'lumot

UC-merced - har bir classi 100 ta tasvirdan iborat bo'lgan 21 ta sinfli quruqlikdagi masofadan zondlash tasvir ma'lumotlari to'plami hisoblanadi. Rasmlar USGS National Map Urban Area Imagery to'plamidan olingan va mamlakatlarning turli shaharlari ustidan qo'lda olingan. Ko'pgina tasvirlar 256x256 piksel bo'lsada, har xil shaklga ega 44 ta rasm mavjud. Dataset parametrlari:

* Versiya: 2.0.0 
* Manba: https://www.tensorflow.org/datasets/catalog/uc_merced
* Manba kodi: tfds.image_classification.UcMerced
* Dataset hajmi: 317.07 MB 

<p align="center">
  <img src="https://github.com/MisterFoziljon/UC-Merced/blob/main/uc_merced-2.0.0.png" />
</p>

#### 2. Loyihani yuklab olish uchun quyidagi ketma-ketlikni bajaring:
  * `windows+R` klavishlarini bosing va paydo bo'lgan oynaga `cmd` buyrug'ini yozing OK tugmachasini bosing.
  
  ![cmd](https://github.com/MisterFoziljon/Fashion-MNIST/blob/main/rasmlar/cmd.png)

  * Loyihani quyidagi link yordamida yuklab oling. (Loyiha uchun yaratilgan fayl adresni o'zingiz ko'rsatishingiz mumkin)

        C:\> git clone https://github.com/MisterFoziljon/CATS_vs_DOGS.git

  * Loyiha joylashgan faylga kiring.
         
        C:\> cd CATS_vs_DOGS


#### 3. Proyektni ishlatish uchun kerakli modullarni virtual environment yaratib o'rnatib oling.
* O'zingizdagi pip ni so'nggi versiyasiga yangilang.

        C:\CATS_vs_DOGS> python -m pip install --upgrade pip
        
* virtual environment yaratish uchun virtualenv modulini o'rnating.
        
        C:\CATS_vs_DOGS> python -m pip install --user virtualenv

* Yangi environment yaratish uchun unga nom bering.
        
        C:\CATS_vs_DOGS> python -m venv sizning_env
        
* Virtual environmentni ishga tushiring(aktivlashtiring).
        
        C:\CATS_vs_DOGS> sizning_env\Scripts\activate.bat
        
* Virtual environment ichiga loyiha ishlashi uchun kerakli bo'lgan modullarni o'rnating (requirements.txt faylining ichida barchasi mavjud).
        
        (sizning_env) C:\CATS_vs_DOGS> pip install -r requirements.txt


#### 4. Proyektni ishlatish uchun jupyter notebook ni ishga tushiring.

        (sizning_env) C:\CATS_vs_DOGS> jupyter notebook
        
  * ```Cats vs Dogs.ipynb``` ni ishga tushiring. 
  * Usbu notebookda [Tensorflow.org](https://www.tensorflow.org/) saytidagi [cats_vs_dogs](https://www.tensorflow.org/datasets/catalog/cats_vs_dogs?hl=ru) datasetini o'qib olish, uni train va test datalariga ajratish, datalarni size va shape larini train uchun moslash hamda normallashtirish ko'rsatilgan. 
  * Dataset yordamida Convolutional Neural Network ishlab chiqilgan va u yordamida model train va evaluate qilingan. Model fayl ko'rinishida saqlanadi. 
  * Notebook yordamida saqlangan modelni load qilish va yangi test qilish datalari yordamida bashorat qilish (predict) ko'rsatib o'tilgan. 
  * [Modelni yuklab olish](https://drive.google.com/drive/folders/1PSvo9ZzQze6EtGdZpZCDCeWM857f6_1I?usp=share_link)
 

#### 5. Proyektni streamlit yordamida deploy qilish.

        (sizning_env) C:\CATS_vs_DOGS> streamlit run streamlit.py

  * Proyekt ```local server```da ishga tushadi va quyidagicha ko'rinishda bo'ladi:


![streamlit1](https://github.com/MisterFoziljon/CATS_vs_DOGS/blob/main/rasmlar/streamlit1.png)
  
  * Rasm faylini yuklab oling va ```Predict``` tugmachasini bosing. Model yuklab olingan tasvirni qaysi turkumga tegishli ekanligini bashorat qiladi. Bundan tashqari softmaxdan chiqqan ehtimollik natijasi ham ekranga chiqadi.


![streamlit3](https://github.com/MisterFoziljon/CATS_vs_DOGS/blob/main/rasmlar/streamlit2.png)
