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
a. Preprocessing <br />
- Gather data training dan testing dengan ukuran gambar 250x250 <br />
- Normalisasi dataset <br />
- Membuat label encoder <br /> 

b. Model 1 <br /> 
- Model menggunakan MaxPooling 2D dan GlobalMaxpooling2D <br />
- Loss = binary cossentropy <br />
- Optimizer = Adam <br />
- Learning rate = 0,0001 <br />
- Epoch = 10 <br />

c. Model 2 <br />
- Model menggunakan AveragePooling2D dan GlobalAveragePooling2D <br />
- Loss = binary cossentropy <br />
- Optimizer = Adam <br />
- Learning rate = 0,0001 <br />
- Epoch = 10<br />
## Modul 3 <br />
a. Preprocessing menggunakan Image Data Generator yang terdiri dari : <br />
- Resize
- Rescaling
- Color Mode
- Shuffle
- Class Mode <br />

b. Model 1 <br />
- Model menggunakan MaxPooling 2D dan GlobalMaxpooling2D <br />
- Menggunakan dropout dan Batch Normalization <br />
- Activation = softmax
- Loss = binary cossentropy <br />
- Optimizer = Adam <br />
- Learning rate = 0,0001 <br />
- Epoch = 100 <br />
- Callback = ReduceLROnplateau <br />

c. Model 2 <br />
- Model menggunakan AveragePooling2D dan GlobalAveragePooling2D <br />
- Menggunakan dropout dan Batch Normalization <br />
- Activation = softmax
- Loss = binary cossentropy <br />
- Optimizer = Adam <br />
- Learning rate = 0,0001 <br />
- Epoch = 100 <br />
- Callback = ReduceLROnplateau <br />

## Modul 4 <br />
a. Preprocessing menggunakan Image Data Generator yang terdiri dari : <br />
- Resize
- Rescaling
- Color Mode
- Shuffle
- Class Mode <br />

b. Model 1 Hparam <br />
- Model menggunakan MaxPooling 2D <br />
- Menggunakan Batch Normalization <br />
- Unit = 32 <br />
- Dropout = 0,2 dan 0,4 <br />
- Activation = softmax <br />
- Loss = categorical cossentropy <br />
- Optimizer = Adam, sgd <br />
- Learning rate = 0,001 <br />
- Epoch = 25 <br />
- Callback = ReduceLROnplateau <br />

c. Model 2 Hparam<br />
- Model menggunakan AveragePooling2D <br />
- Menggunakan Batch Normalization <br />
- Unit = 64 <br />
- Dropout = 0,3 dan 0,5 <br />
- Activation = softmax <br />
- Loss = categorical cossentropy <br />
- Optimizer = Adam dan Adadelta <br />
- Learning rate = 0,0001 <br />
- Epoch = 25 <br />
- Callback = ReduceLROnplateau <br />
