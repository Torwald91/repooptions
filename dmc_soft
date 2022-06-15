#!/usr/bin/python3

import os
import sys


print('**************Welcome User!***************')

print('')
print('1. Продолжить')
print('2. Выход')
print('')
otv = int(input('Введите число --> '))
print('')

#Фунционал ПО
def Update():
	os.system('apt update && apt full-upgrade -y')
def Remove():
	os.system('apt autoremove')
def Create():
	print('--------------Menu--------------')
	print('')
	print('1. Создать папку')
	print('2. Создать файл')
	print('')
	cr = int(input('Введите число --> '))
	if cr == 1:
		name_d = input('Введите путь и имя папки (Пример: /home/user/имя_папки, ~/имя_папки) --> ')
		os.system('mkdir '+ name_d)
	if cr == 2:
		name_f = input('Введите путь и имя файла (Пример: /home/user/имя_файла, ~/имя_файла) --> ')
		os.system('touch '+ name_f)
	else:
		pass

def CreateARH():
	putarh = input('Введите путь (что нужно архивировать) --> ')
	namearh = input('Введите путь и имя архива (где он будет хранится) --> ')
	os.system(f'tar -cvjf {namearh}.tar.bz {putarh}')

def Main():
	while otv == 1:
		print('++++++++++++++Menu++++++++++++++')
		print('')
		print('1. Обновить ситемы')
		print('2. Удалить старые пакеты')
		print('3. Создать папку или файл')
		print('4. Создать архив')
		print('0. Выход')
		print('')
		sys_proc = int(input('Введите число -->> '))
	
		if sys_proc == 1:
			Update()
		elif sys_proc == 2:
			Remove()
		elif sys_proc == 3:
			Create()
		elif sys_proc == 4:
			CreateARH()
		else:
			print('')
			print('Bye')
			print('')
			break
	else:
		print('Bye')
		print('')

Main()
print('HELLO')
