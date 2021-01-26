# QR-Code-generator
Creating a QR Code using Python that will redirect you to a specified URL.

!pip install pyqrcode
!pip install pypng

#Create a QR Code that will redirect to my Linkedin Profile

import pyqrcode
import png
from pyqrcode import QRCode

#String represents the QR Code
site = "https://www.linkedin.com/in/come2ayush/"

#Generate QR Code
url = pyqrcode.create(site)

# Create and display the QR Code in PNG format
url.png("MyProfile.png", scale = 6)
url.show()
