# qr-code-project
import qrcode
#for generating qrcode for messages
qr=qrcode.make("qr code generator project ")
qr.save("mes_qr.png")
qr.show()

#for generating qrcode for links
link="https://www.youtube.com/"
qr=qr.make(link)
qr.save("linkqy.png")
qr.show()
#for generating qrcode for personal deatails
qr=qrcode.QRCode
       {
           version=5
           box_size=2
           border=2
       }
name=input("enter a name:")
age=int(input("enter age:"))
mobile=int(input("enter mobile number:"))
data={"Name":name,"Age":age,"Mobile":mobile}
qr.add_data(data)
qr.make(fit=True)
img=qr.make_image()
img.save("per_qr.png")
img.show()






