# TugasPraktikumML_058-082
Anggota Kelompok : <br />
Tsabita Nurul Izzah - 201810370311082 <br />
Ulfa Zakiatul Mardhiah - 201810370311058 
## Sumber Referensi <br />
Dataset           : https://www.kaggle.com/iarunava/cell-images-for-detecting-malaria  <br />
Artikel Rujukan   : http://dx.doi.org/10.26760/elkomika.v9i2.306 <br />
## Dataset <br />
Dataset yang digunakan terdiri dari 27.558 gambar slide apusan darah tipis dari Malaria Screener research activity. Dataset tersebut terbagi menjadi 2 kategori yaitu gambar sel dengan contoh yang sama dari sel yang terjangkit parasit(Parasitized) dan tidak terinfeksi(Uninfected). 
## Modul 2 <br />
Preprocessing <br />
1. Gather data training dan testing dengan ukuran gambar 250x250 <br />
2. Normalisasi dataset <br />
3. Membuat label encoder <br />
*Model 1 <br />
1. Model menggunakan MaxPooling 2D dan GlobalMaxpooling2D <br />
2. Loss = binary cossentropy <br />
3. Optimizer = Adam <br />
4. Learning rate = 0,0001 <br />
5. Epoch = 10 <br />
*Model 2 <br />
1. Model menggunakan AveragePooling2D dan GlobalAveragePooling2D <br />
2. Loss = binary cossentropy <br />
3. Optimizer = Adam <br />
4. Learning rate = 0,0001 <br />
5. Epoch = 10<br />
## Modul 3 <br />
Preprocessing menggunakan Image Data Generator yang terdiri dari : <br />
1. Resize
2. Rescaling
3. Color Mode
4. Shuffle
5. Class Mode
*Model 1 <br />
1. Model menggunakan MaxPooling 2D dan GlobalMaxpooling2D <br />
2. Menggunakan dropout dan Batch Normalization <br />
3. Activation = softmax
4. Loss = binary cossentropy <br />
5. Optimizer = Adam <br />
6. Learning rate = 0,0001 <br />
7. Epoch = 100 <br />
8. Callback = ReduceLROnplateau <br />
*Model 2 <br />
1. Model menggunakan AveragePooling2D dan GlobalAveragePooling2D <br />
2. Menggunakan dropout dan Batch Normalization <br />
3. Activation = softmax
4. Loss = binary cossentropy <br />
5. Optimizer = Adam <br />
6. Learning rate = 0,0001 <br />
7. Epoch = 100 <br />
8. Callback = ReduceLROnplateau <br />
