#generador qr en python 
from qrcode import make 

class QrCode():
    def __init__(self):
        self.image = make(input(" Enlace Qr : ")) 
        self.qr_name = input(" Nombre del archivo ") 

    def save(self):  
        self.image.save(self.qr_name)

    def show(self):  
        self.image.show(self.qr_name)



if __name__ == '__main__':
    qr = QrCode()
    qr.save()
    qr.show()

