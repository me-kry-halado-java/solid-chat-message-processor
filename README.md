# solid-chat-message-processor

chat uzenet feldolgozo osztaly keszitese.

ChatMessage.process(String message) metodus
Ez vegighivja az osszes feldolgozot, es igazzal ter vissza, ha mindenki fel tudta dolgozni.
legyen 3 feldolgozo:
- ideiglenes tarolo: memoriaban tarolja a kapott logokat (masik metodussal majd visszaadja)
- statisztika: tarolja el, hogy hany szo, mondat, betu (masik metodussal majd visszaadja)
- muveleti feldolgozo: speci tartalmat keres. most egy parancsot ismer a \m:from:to:mess email uzenet kuldese.
   - EmailSender interface a fuggosege, amit meghiv, ha megtalalta a mintat.

Csak service osztalyok es a tesztek kellenek. Kimenete egy jar file.
