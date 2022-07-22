# TF2-Linear-Regression

![image](https://user-images.githubusercontent.com/87703066/180495303-191ac0f5-7278-498a-b0ff-799a614105ac.png)


Pembuatan model linear regresi dengan menggunakan tensorflow v2

Langkah-langkah yang digunakan:

1. Import data yang digunakan (sumber data : https://raw.githubusercontent.com/lazyprogrammer/machine_learning_examples/master/tf2.0/moore.csv)

2. Tentukan variabel X dan Ynya

3. Plot variabel X dan Y

![image](https://user-images.githubusercontent.com/87703066/180458067-759fef88-18a9-4be0-bb03-d81e29d2f059.png)

4. Karena kita ingin menggunakan linear regresi maka gunakan log. penggunaan log diperlukan untuk memenuhi hubungan linear regresi. plot lagi variabel X dan Y

![image](https://user-images.githubusercontent.com/87703066/180458372-c8bbd29a-1072-4e08-911f-6888aa35a125.png)

5. Skalakan nilai X agar tidak terlalu besar, namun nanti kita harus mengubahnya lagi

6. Buat model
- 2 Layer : input dan dense 
- optimizer menggunakan SGD

#### GD VS SGD

Gradient Descent, atau GD menggunakan nilai learning rate yang kecil. GD akan melakukan update weights setelah semua data training harus selesai diproses, atau setiap 1 epoch (iterasi). Karena learning rate yang kecil maka untuk mencapai minimum dibutuhkan proses yang lama.

Stochastic Gradient Descent (SGD) adalah solusi untuk menyelesaikan issue dari GD. SGD akan melakukan update weight tanpa menunggu 1 epoch selesai. SGD menggunakan konsep yang mirip dengan batching dengan membagi data training menjadi beberapa batch. Weight akan diupdate dalam setiap batch selesai diproses.

![image](https://user-images.githubusercontent.com/87703066/180459459-a54a43a4-a595-4a8f-b9da-acad999e1152.png)

(sumber : https://skillplus.web.id/gradient-descent-dan-learning-rate-lanjutan/ )


7. Menentukan learning rate . Setting fungsi untuk epoch diatas 50 maka learning rate akan turun

![image](https://user-images.githubusercontent.com/87703066/180460759-561f88ee-e260-4c53-b739-5d51436aa34d.png)

8. Melihat nilai w dan b

![image](https://user-images.githubusercontent.com/87703066/180461154-86a14b09-454c-4e02-b3fa-3f4ee252e6af.png)


