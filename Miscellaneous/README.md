# sanity_check
> Here is your flag: 466f726573747948437b77656c636f6d655f746f5f6861636b65725f636c6173735f666f72657374795f3539366537377d0a

## About the Challenge
Diberikan sebuah pola berupa angka-angka dan huruf random dengan asumsi bilangan ascii seperti gambar dibawah ini.

![pic1](images/pic1.jpg)

## Solution
Soal diatas merupaka soal kriptografi yang diasumsikan dengan bentuk pola hexadesimal. Penyelesaian kode ini dapat dilakukan dengan banyak cara, salah satunya dengan membuat codingan dalam bahasa python. Saya telah membuat kodenya seperti dibawah ini dengan menggunakan library binascii dan konversi string hexadecimal dengan kode bytes.fromhex(hex_str).decode('utf-8'). Kode ini akan menghasilkan hasil keluaran berupa string yang didekripsi dari rangkaian karakter heksadesimal yang diberikan.

```shell
import binascii

hex_str = "466f726573747948437b77656c636f6d655f746f5f6861636b65725f636c6173735f666f72657374795f3539366537377d0a"
byte_str = bytes.fromhex(hex_str).decode('utf-8')
print(byte_str)

```

```
ForestyHC{welcome_to_hacker_class_foresty_596e77}
```