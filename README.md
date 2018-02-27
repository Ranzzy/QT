# Лабораторная работа №8  Использование фреймворка Qt для разработки графического приложения
<b>Цель работы:</b> разработать на языке C++ с использованием кросплатформенного фреймворка с открытым исходным кодом Qt графическое приложение.<p>

<b>Qt</b> — это кроссплатформенный инструмент с открытым исходным кодом для разработки программ на языке программирования С++.<p>

<b>Ход работы:</b><p>
Сначала обновите список пакетов:<br>
 <i>sudo apt-get update</i><br>

Теперь, чтобы установить Qt выполните:<br>
 <i>sudo apt-get install qt5-default</i><br>

Если вам также нужна установка QtCreator, то это сделать тоже не так сложно:<br>
 <i>sudo apt-get install qtcreator</i><br>

И установите примеры программ на qt5 если это нужно:<br>
 <i>sudo apt-get install qtbase5-examples qtdeclarative5-examples</i><br><p>

Далее был прописан код в main.cpp:<br>

<i>#include <QApplication><br>
#include <QMainWindow><br>
#include <QDesktopWidget><br>
#include <QMenuBar><br>

int main(intargc, char *argv[])
{<br>
QApplicationa(argc, argv);<br>
QMainWindow w;<br>
QMenu *fileMenu = w.menuBar()->addMenu("&File");<br>

QDesktopWidgetdw;<br>
int x=dw.width()*0.7;<br>
int y=dw.height()*0.7;<br>
w.setFixedSize(x,y);<br>
w.show();<br>
returna.exec();<br>
}<br></i>
И созданы файлы сборки и запуска программы.<p>
<b>Вывод:</b> на практическом занятии, используя среду разработки Visual Studio Code было написано простое QT приложение состоящее из нескольких элементов интерфейса.