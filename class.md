# **Class dan Object**

```
class ClassName:
    <statement-1>
    .
    .
    .
    <statement-N>
```

```py
class classx:
    variable = "Ini contoh class"

    def myFunc(self):
        return "Ini function di dalam class"

clss = classx()
print(clss.variable) #output Ini contoh class
print(clss.myFunc()) #output Ini function di dalam class
```

```py
class bangunRuang:
    def __init__(self, panjang, lebar, alas, tinggi, sisi, sisiMiring, jari):
        self.panjang = panjang
        self.lebar = lebar
        self.alas = alas
        self.tinggi = tinggi
        self.sisi = sisi
        self.pi = 3.15
        self.jari = jari
        self.sisiMiring = sisiMiring

    def luasPersegiPanjang(self):
        return self.panjang * self.lebar

    def kelilingPersegiPanjang(self):
        return 2*(self.panjang + self.lebar)

    def luasPersegi(self):
        return self.sisi**2

    def kelilingPersegi(self):
        return 4 * self.sisi

    def luasLingkaran(self):
        return self.pi * self.jari**2

    def kelilingLingkaran(self):
        return 2 * self.pi * self.jari

    def luasSegitigaSikuSiku(self):
        return 0.5 * self.alas * self.tinggi

    def kelilingSegitigaSikuSiku(self):
        return self.sisiMiring + self.alas + self.tinggi


#Deklarasi nilai variabel dalam satuan cm
panjang = 20
lebar = 30
alas = 10
tinggi = 10
sisi = 5
sisiMiring = 3
jari = 3

# pemanggilan class bangun ruang
hitung = bangunRuang(panjang, lebar, alas, tinggi, sisi, sisiMiring, jari)

print("Panjang dari persegi panjang = %d cm dan lebar %d cm" %(hitung.panjang, hitung.lebar)) 
print("Luas persegi panjang = %f cm"%hitung.luasPersegiPanjang())
print("Keliling persegi panjang = %f cm"%hitung.kelilingPersegiPanjang())
print("Luas persegi = %f cm"%hitung.luasPersegi())
print("Keliling persegi = %f cm"%hitung.kelilingPersegi())
print("Luas lingkaran = %f cm"%hitung.luasLingkaran())
print("Keliling lingkaran = %f cm"%hitung.kelilingLingkaran())
print("Luas segitiga siku-siku = %f cm"%hitung.luasSegitigaSikuSiku())
print("Keliling segitiga siku-siku = %f cm"%hitung.kelilingSegitigaSikuSiku())

# Panjang dari persegi panjang = 20 cm dan lebar 30 cm
# Luas persegi panjang = 600.000000 cm
# Keliling persegi panjang = 100.000000 cm
# Luas persegi = 25.000000 cm
# Keliling persegi = 20.000000 cm
# Luas lingkaran = 28.350000 cm
# Keliling lingkaran = 18.900000 cm
# Luas segitiga siku-siku = 50.000000 cm
# Keliling segitiga siku-siku = 23.000000 cm
```



