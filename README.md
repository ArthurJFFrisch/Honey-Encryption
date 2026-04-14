# Honey-Encryption
Die Grundidee dder Honey-Encryption ist auf Wikipedia zu finden: https://de.wikipedia.org/wiki/Honey_Encryption
In diesem Projekt möchte ich selbst versuchen eine möglichst gute Honey-Encryption zu erstellen.
## Ziele
- die Fake-Daten müssen Inhaltlich passend sein, dürfen allerdings nicht die vertraulichen Informationen preisgeben
- Bestimmte Phrasen oder Wörter, von denen ein möglicher Angreifer weis, dass sie enthalten sind müssen auch in den Fake-Daten enthalten sein
## Grundstruktur
- Klartext wird in Tokens umgewandelt
- Mithilfe eines GPT Modelles wird die Wahrscheinlichkeit jedes Tokens des Klartextes berechnet
- Diese Wahrscheinlichkeiten werden mit einer herkömmlichen Verschlüsselung verschlüsselt
- Die neu entstandenen Wahrscheinlichkeiten werden in ein GPT eingespeist, welches neue Tokens generiert
- Diese werden zu einem verschlüsselten Text zusammengesetzt, der dennoch plausibel erscheint
