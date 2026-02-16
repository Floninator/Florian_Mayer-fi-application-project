# -*- coding: utf-8 -*-
import random
zufallsantworten=["Jaja", "Ich check", "Okay, wenn du nicht willst dann lass", "Reicht jetzt auch, ne?", "Fragst du dich vielleicht wie ich funktioniere", "Ich programmiere gerne!"]
reaktionsantworten = {"hallo": "aber Hallo", 
                      "geht": "Was verstehst du darunter?", 
                      "essen": "Ich bin Sinnlos :(", 
                      "lernen": "Ich bin ein Bot", 
                      "mathe": "1+1=11",
                      "hobbys": "Sport, Musik produzieren und Klavier spielen, Reisen und natürlich programmieren lernen:)",
                      "schätzt": "Freundlichkeit :)",
                      "funktionierst": "Ich bin ein Python Projekt mit folgenden Funktionen: Verarbeitung von Nutzereingaben, Erkennung von Schlüsselwörtern und individuelle                                  Reaktionen, zufällige Antworten durch 'random' und Dictionary, Nutzung von while-Schleifen.", 
                      "wie": "Ich bin ein Python Projekt mit folgenden Funktionen: Verarbeitung von Nutzereingaben, Erkennung von Schlüsselwörtern und individuelle                                            Reaktionen, zufällige Antworten durch \"random"\ und Dictionary, Nutzung von while-Schleifen.",
                      "danke": "gerne"}
print("Dieses Projekt entstand zur Vorbereitung auf eine Ausbildung zum Anwendungsentwickler. Es zeigt meinen Einstieg in die Programmierung, sowie meine Motivation, mir IT-Kenntnisse eigenständig anzueignen. Dieses Projekt befindet sich bewusst im Aufbau, da es hier um den Lernprozess geht und nicht um fertige Projekte.")                      
print("Hey")
print("Worüber würden Sie gerne heute sprechen?")
print("Zum Beenden einfach 'bye' eintippen")
print("")

nutzereingabe = ""
while nutzereingabe != "bye" :
  nutzereingabe = ""
  while nutzereingabe == "":
     nutzereingabe = input("Ihre Frage/Antwort: ")
     
  nutzereingabe = nutzereingabe.lower()
  nutzerwoerter = nutzereingabe.split()

  intelligenteAntworten = False
# print(nutzerwoerter)
  for einzelwoerter in nutzerwoerter:
    if einzelwoerter in reaktionsantworten:
      print(reaktionsantworten[einzelwoerter])
      intelligentAntworten = True
  if intelligenteAntworten == False:
    print(random.choice(zufallsantworten))

  print("")
  
print("Gerneschön und auf wiedersehen")
exit()


