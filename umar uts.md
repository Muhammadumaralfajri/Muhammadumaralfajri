# 1.

```py
jml = 5
nama_list = []
nilai_list = []
for lis in range(1, jml+1):
    nama = str(input(f"Input nama ke {lis} : "))
    nama_list.append(nama)
    nilai = int(input(f"Input nilai ke {lis} : "))
    nilai_list.append(nilai)
    print()
   
print(f"""
      ========================================================================
        No     nama              Nilai
      ========================================================================
      """)

for hasil in range(1, jml+1):
    print(f"       {hasil}      ", nama_list[hasil-1],"                ", nilai_list[hasil-1])
    

print(f"""
      ========================================================================
        Jumlah mahasiswa : {jml}
        Rata-rata : {sum(nilai_list)/jml}
      """)

```
![image](https://user-images.githubusercontent.com/93040764/142467899-21392b2d-68d8-4e7b-bea3-638e18442070.png)

# 2.
```py
jml = 5
nama_list = []
nilai_list = []
ket_list = []

for lis in range(1, jml+1):
    nama = str(input(f"Input nama ke {lis} : "))
    nama_list.append(nama)
    nilai = int(input(f"Input nilai ke {lis} : "))
    nilai_list.append(nilai)
    print()
    if nilai_list[lis-1] >=60:
      ket = "Lulus"
    else:
      ket = "Tidak Lulus"
    ket_list.append(ket)  

print(f"""
      ========================================================================
        No     nama              Nilai                Keterangan
      ========================================================================
      """)
maxim = max(nilai_list)
minim = min(nilai_list)
for hasil in range(1, jml+1):
    print(f"       {hasil}      ", nama_list[hasil-1],"              ", nilai_list[hasil-1],"            ",ket_list[hasil-1])
    
print(f"""
      ========================================================================
        Jumlah mahasiswa    = {jml}
        Rata-rata           = {sum(nilai_list)/jml}
        Nilai tertinggi     = {max(nilai_list)} oleh {nama_list[nilai_list.index(maxim)]}
        Nilai tertinggi     = {min(nilai_list)} oleh {nama_list[nilai_list.index(minim)]}
        Jumlah lulus        = {ket_list.count("Lulus")}
        Jumlah gagal        = {ket_list.count("Tidak Lulus")}
      """)

```
![image](https://user-images.githubusercontent.com/93040764/142469473-30ba96ab-a993-4bb5-b05f-a3c245759371.png)

# 3.
```py
listnama = []
listtugas = []
listuts = []
listuas = []
na = []
jumlah = int(input("Masukkan jumlah mahasiswa : "))

for i in range(1, jumlah+1):
    nama = str(input("Masukkan nama : "))
    listnama.append(nama)
    tugas = float(input("Masukkan nilai tugas : "))
    listtugas.append(tugas)
    uts = float(input("Masukkan nilai uts : "))
    listuts.append(uts)
    uas = float(input("Masukkan nilai uas : "))
    listuas.append(uas)
    na.append(0.30*tugas+0.30*uts*0.40*uas)
    print()
print("-------------------------------------------------------------------")
print("No       Nama      Tugas        UTS         UAS      Nilai Akhir")
print("-------------------------------------------------------------------")

for nilai in range(1, jumlah+1):
    print(
        f"{nilai}        {listnama[nilai-1]}      {listtugas[nilai-1]}        {listuts[nilai-1]}        {listuas[nilai-1]}      {na[nilai-1]}")
print("-------------------------------------------------------------------")

ratatugas = sum(listtugas)/jumlah
ratauts = sum(listuts)/jumlah
ratauas = sum(listuas)/jumlah
ratana = sum(na)/jumlah
print(f"Rata-rata       {ratatugas}     {ratauts}       {ratauas}       {ratana}")
print("-------------------------------------------------------------------")

```
![image](https://user-images.githubusercontent.com/93040764/142470730-3a086315-071d-4633-ab15-9bd8362f0e01.png)

# 4.
  ```py
  bilangan = []


for i in range(0, 5):
   data = int(input("Masukkan bilangan "))
   bilangan.append(data)
   
for num in bilangan:
    if num %2 == 0:
        print(num, end=" ")
  
  ```
  ![image](https://user-images.githubusercontent.com/93040764/142471809-bd993a84-adb8-4a8d-bdc7-015ccb8b4ec4.png)

# 5.
```py
big = [80, 100, 50, 70, 90, 99, 40, ]
print(max(big))


```
![image](https://user-images.githubusercontent.com/93040764/142472383-c0337c1c-33e5-43d1-b908-835684ee8a1e.png)

# 6.
```py
indeks1 = []
indeks2 = []
indeks3 = []
indeks4 = []

newin1 = []
newin2 = []
newin3 = []
newin4 = []
1
for i in range(0, 5):
    data = int(input("Masukkan data untuk ketentuan A  "))
    indeks1.append(data)
    if i == 5:
     print()


for a in indeks1:
    if a %2 == 0:
        newin1.append(a)
print("Data yang berindeks genap saja = ", " ".join(map(str, newin1)))

for i in range(0, 5):
    data = int(input("Masukkan data untuk ketentuan B :  "))
    indeks2.append(data)
    if i == 5:
     print()


for b in indeks2:
    if b   >= 0:
        newin2.append(b)


print("Data yang bernilai positif saja = ")
print(" ".join(map(str, newin2)))

for i in range(0, 5):
    data = int(input("Masukkan data untuk ketentuan C :  "))
    indeks3.append(data)
    if i == 5:
     print()


for c in indeks3:
    if c %3 == 0 and c %2 != 0 :
        newin3.append(c)


print("Data Bilangan ganjil yang kelipatan 3 saja = ")
print(" ".join(map(str, newin3)))

for i in range(0, 5):
    data = int(input("Masukkan data untuk ketentuan d :  "))
    indeks4.append(data)
    if i == 5:
     print()


for d in indeks4:
    if d % 3 != 0:
        newin4.append(d)


print("Data Bilangan yang tidak habis dibagi 3 = ")
print(" ".join(map(str, newin4)))



```
![image](https://user-images.githubusercontent.com/93040764/142472964-22e89aea-1e3e-4d64-bd3a-cbb562427d55.png)

# 7.
```py
kelipatan = 5

total = []

for i in range(0, 10):
    data = int(input("Masukkan data : "))
    if data % kelipatan == 0:
        total.append(data)
        

print("Kelipatan 5 pada list terdapat sebanyak", len(total))
for i in total:
    print(i, end=" ")


```
![image](https://user-images.githubusercontent.com/93040764/142473537-01a5909a-ab80-402d-8c7f-5d385cc84c07.png)

# 8.
```py


```

# 9.
```py
num = []

for i in range(0, 5):
    data = int(input("Masukkan bilangan : "))
    num.append(data)
    
print(f"Jumlah bilangan dalam list = {sum(num)}")
occur = max(set(num), key=num.count)
print("Data yang paling sering di input = ", occur)


```
![image](https://user-images.githubusercontent.com/93040764/142474227-5f372aea-6b31-4a2a-ba27-1241129170f4.png)

# 10.
```py
j = []
p = ""
n = ""
for i in range(0, 5):
    data = int(input("Masukkan bilangan : "))
    j.append(data)
    
for num in j:
    if num >=0:
        p =+1
    else:
        n =+1
        
if p > n:
    print("Positive lebih banyak")
else:
    print("Negative lebih banyak")


```
![image](https://user-images.githubusercontent.com/93040764/142474823-2796dd59-021d-4a3f-8e85-30b912cbe9dd.png)

# 11.
```py


```

# 12.
```py
a = (1,2,3,4,5)
perkalian = int(input("Masukkan angka untuk dikalikan dengan tuple : "))
for tup in a:
    print(f"{perkalian} * {tup} = {perkalian*tup}")


```
![image](https://user-images.githubusercontent.com/93040764/142475221-807210a4-b4ad-411c-9bf1-eb716951606a.png)

# 13.
```py
dict1 = {
    "nim":"1235678",
    "nama":"umar",
    "IPK":3.90,
}
dict2 = {
    "Hobi":"Futsal",
    "alamat":"bandung"
}

dict1.update(dict2)

for x, y in dict1.items():
    print(f"{x} : {y}")


```
![image](https://user-images.githubusercontent.com/93040764/142475780-f22ec2b8-4fc1-47f8-a59f-573f88f50b6c.png)


