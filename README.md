def faktoriyel(sayi):
    faktoriyel = 1        
    if sayi == 1 or sayi == 0:
        return faktoriyel  # 0! ve 1! her zaman 1'dir
    else:
        while sayi >= 1:
            faktoriyel *= sayi
            sayi -= 1
        return faktoriyel  # Döngü tamamlandıktan sonra sonucu döndür

try:
    sayi = int(input("Bir sayı girin: "))  # Kullanıcıdan bir sayı alın
    if sayi < 0:
        print("Negatif sayıların faktöriyeli hesaplanamaz.")
    else:
        sonuc = faktoriyel(sayi)
        print("Faktöriyel:", sonuc)
except ValueError:
    print("Lütfen geçerli bir tam sayı girin.")
