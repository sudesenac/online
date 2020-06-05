#!/usr/bin/python
# -*- coding: utf-8 -*-

def hesaplama(talep,cevap):
	uzunluk = len(cevap)
	i=0
	toplamCevap=0
	while i!=uzunluk:
		if cevap[i]==1:
			toplamCevap+=1
		i+=1
	return toplamCevap*1.0/uzunluk

talep=[]
cevap=[]
yuzde=0

while yuzde<0.8:
	talep.append(int(input("Talep girişini yapınız: ")))
	cevap.append(int(input("Cevap girişini yapınız: ")))
	yuzde=hesaplama(talep,cevap)
	print("Taleplere verilen cevap oranı: "+ str(yuzde))

