# Robo-speaker
import win32com.client as wincom
# you can insert gaps in the narration by adding sleep calls
#import time
speak = wincom.Dispatch("SAPI.SpVoice")
print("welcome to RoboSpearker 1.1. Created by Robin")
while True:
    x =input("Enter what you want me to speak")
    if x == "q":
        speak.Speak("bye bye friend see u")
        break
    speak.Speak(x)
                
