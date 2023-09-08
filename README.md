# Text-To-Speech
With the help of gtts library, i'll convert text to speech in diff-2 languages . 



import gtts
import playsound
w=['a.mp3','b.mp3','c.mp3','d.mp3','e.mp3','f.mp3','g.mp3','h.mp3','i.mp3','j.mp3','k.mp3']
for i in range(len(w)):
    p=input("W")
    if p=='q':
        break
    s=gtts.gTTS(p, lang='hi')
    s.save(w[i])
    playsound.playsound(w[i])
