# python

#아나콘다를 활용하여 계산기를 구현.

#python code:
import sys
from PyQt5.QtWidgets import *
from PyQt5 import uic

ui_path = "test1.ui"
form_class = uic.loadUiType(ui_path)[0]

class WIndowClass(QMainWindow, form_class):
    def __init__(self):
        super().__init__()
        self.setupUi(self)

if __name__ == "__main__":
    app = QApplication(sys.argv)
    myWindow = WIndowClass()
    myWindow.show()
    app.exec_()
    
아나콘다 ui :

<img width="278" alt="k" src="https://user-images.githubusercontent.com/79035077/194743634-f0a6816d-9c26-4bbf-821c-801b64dc2067.png">
