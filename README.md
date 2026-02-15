# Florian_Mayer-fi-application-project
Dieses Projekt entstand zur Vorbereitung auf eine Ausbildung zum Anwendungsentwickler. Es zeigt meinen Einstieg in die Programmierung, sowie meine Motivation, mir IT-Kenntnisse eigenständig anzueignen. Dieses Projekt befindet sich bewusst im Aufbau, da es hier um den Lernprozess geht und nicht um fertige Projekte.
# -*- coding: utf -*-
import random
zufallsantworten=["Jaja", "Ich check", "Okay, wenn du nicht willst dann lass", "Reicht jetzt auch, ne?"]
reaktionsantworten = {"hallo": "aber Hallo", 
                      "geht": "Was verstehst du darunter?", 
                      "essen": "Ich bin Sinnlos :(", 
                      "lernen": "Ich bin ein Bot", "mathe": "1+1=11"}
print("Hey")
print("Worüber würden Sie gerne heute sprechen?")
print("Zum Beenden einfach 'bye' eintippen")
print("")

nutzereingabe = ""
while nutzereingabe != "bye" :
  nutzereingabe = ""
  while nutzereingabe = "":
     nutzereingabe = input("Ihre Frage/Antwort: ")
     
  nutzrereingabe = nutzereingabe.lower()
  nutzerwoerter = nutzereingabe.split()

  intelligenteAntworten = False
# print(nutzerwoerter)
  for einzelwoerter in nutzerwoerter:
    if einzelwoerter in reaktionsantworten:
      print(reaktionsantworten[einzelwoerter])
      intelligentAntworten = True
  if intelligenteAntworten = False:
  print(random.choice(zufallsantworten))

  print("")
  
print("Gerneschön und auf wiedersehen")
exit()


