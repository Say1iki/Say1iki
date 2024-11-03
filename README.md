class Calisan:
    def __init__(self, isim, maas, departman):
        print("Çalışan sınıfı init fonksiyonu")
        
        self.isim = isim
        self.maas = maas
        self.departman = departman
        print("Çalışan sınıf bilgileri")
        print("İsim: {} \nMaaş: {} \nDepartman: {}\n".format(self.isim, self.maas, self.departman))

    def departman_degistir(self, yeni_departman):
        self.departman = yeni_departman
        print("Departman değiştirildi: {}".format(self.departman))


class Yönetici(Calisan):
    pass
yonetici = Yönetici("Mustafa Murat Coşkun", 300, "Bilişim")

