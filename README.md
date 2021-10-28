# BarcodeGenerator
import barcode
from barcode.writer import ImageWriter

text = "Python Programming"
text1 = str(text)
code = barcode.get_barcode_class("code128")
image = code(text, Writer=ImageWriter())
save_img = image.save('Final Barcode#name of barcode to be saved as')
