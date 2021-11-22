# Project CNN
# Klasifikasi Penyakit Jagung melalui Citra Daun Menggunakan Algoritma Convolutional Neural Network


Daftar Anggota :
1. Putra Prassiesa Abimanyu (E41192178)
2. Bagus Bachtiar Rizki (E41192340)
3. Mita Unziyah Fajrina (E41192433)
4. Devan Ferdiansyah (E41191971)
5. Sofyan Arif Af Rizal (E41192160)

##
## Dataset Description:<br>
0: Common Rust - 300 images <br>
1: Gray Leaf Spot - 300 images <br>
2: Blight - 300 images <br>
3: Healthy - 300 images

## Note: <br>
This dataset has been made using the popular PlantVillage and PlantDoc datasets. During the formation of the dataset certain images have been removed which were not found to be useful.

##
## Best Test Score <br>
<img src="https://github.com/ppabimanyu/Tugas---CNN/blob/master/src/img.png" width="50%">
<br>
##
<img src="data:image/png;base64,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" width="100%">


