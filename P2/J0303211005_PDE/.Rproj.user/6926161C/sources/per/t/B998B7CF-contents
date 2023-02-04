#1.    Hitung statistika deskriptif dari dataset iris dan interpretasikan outputnya untuk variable:

#Petal Length
#perintah summary berfungsi untuk menampilkan nilai ringkasan dari Petal.Length
summary(iris$Petal.Length)
#karena dalam perintah summary tidak terdapat nilai modus, maka kita cari secara manual, dengan mengetikkan perintah-perintah di bawah iniL:
table(iris$Petal.Length)
#perintah manual untuk mencari nilai modus atau nilai yang paling banyak dalam data Petal Length
modus <- names(table(iris$Petal.Length))[table(iris$Petal.Length)==max(table(iris$Petal.Length))]

print(paste("Modus dari Petal Length adalah", modus))

#Petal Width
#perintah summary berfungsi untuk menampilkan nilai ringkasan dari Petal Width
summary(iris$Petal.Width)
#karena dalam perintah summary tidak terdapat nilai modus, maka kita cari secara manual, dengan mengetikkan perintah-perintah di bawah ini:
table(iris$Petal.Width)
#perintah manual untuk mencari nilai modus atau nilai yang paling banyak dalam data Petal Width
modus <- names(table(iris$Petal.Width))[table(iris$Petal.Width)==max(table(iris$Petal.Width))]

print(paste("Modus dari Petal Length adalah", modus))

#2.    Hitung nilai ukuran dispersi untuk variable Petal.Length pada dataset iris
quantile(iris$Petal.Length, 0.25)
quantile(iris$Petal.Length, 0.75)

IQR(iris$Petal.Length)
iqr <- as.vector(quantile(iris$Petal.Length))
iqr[4]-iqr[2]

sd(iris$Petal.Length)
var(iris$Petal.Length)
lapply(iris[,1:4], sd)
lapply(iris[,1:4], var)
summary(iris)

#3.    Hitung kurtosis dan skewness dari variable Petal.Width pada dataset iris
library(moments)
skewness(iris$Petal.Width)
kurtosis(iris$Petal.Width)

#4.    Hitung matrix korelasi pada dataset iris, interpretasikan outputnya dan visualisasikan hasilnya
library(corrplot)
round(cor(iris[,1:4]), digits=2)
corrplot(cor(iris[,1:4]),method="number",type="upper")

#5.    Berikut data tentang jumlah pengunjung XXI hari ke-20 s.d hari ke-49. Buat tabel distribusi frekuensinya dan bagi kelas interval sesuai dengan yang Anda inginkan.
#Buat tabel distribusi frekuensinya dan bagi kelas interval sesuai dengan yang Anda inginkan.

baris1<-c(67,87,67,54,67)
baris2<-c(86,76,100,56,45)
baris3<-c(78,44,90,89,78)
baris4<-c(77,86,45,67,77)
baris5<-c(99,60,87,87,112)
baris6<-c(45,56,78,65,67)

nilai<-c(baris1,baris2,baris3,baris4,baris5,baris6)
sort(nilai)

length(nilai)

cut(nilai,breaks=3)

table(cut(nilai,breaks=3))

cbind(table(cut(nilai,breaks=3)))

cut(nilai,breaks=seq(43.5,112.5,10))

table(cut(nilai,breaks=seq(43.5,112.5,10)))

cbind(table(cut(nilai,breaks=seq(43.5,112.5,10))))

# dapat juga menggunakan fungsi transfor()
transform(table(cut(nilai,breaks=seq(43.5,112.5,10))))

#6.    Jalankan R atau RStudio kemudian ketikkan skrip berikut:
pairs(~Sepal.Length+Sepal.Width+Petal.Length+Petal.Width,
      data = iris,
      lower.panel = NULL,
      main="Simple Scatter Plot Matrix")
#7.    Buat diagram dahan dauh(*Steam and Leaf Plot*) untuk data diatas
stem(nilai)
