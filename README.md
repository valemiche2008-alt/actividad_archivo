# actividad_archivo
*import json

name = input("cual es tu nombre?: ")
clan = input("cual es tu clan?: ")

route = "./data/coders.json"

#crear o escribir .
try:
    
    with open("route", "w", newline="", encoding="utf-8" ) as filecoders:
        json.dump({ 1: {"name": name , "clan": clan }}, filecoders, indent=4)


    #leer data 
    with open("route", "r", newline="", encoding="utf-8" ) as filecoders:
        readed = json.load(filecoders)
    print(readed)**
