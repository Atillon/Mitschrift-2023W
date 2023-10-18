
17.10.2023

Notiz: erste stunde fehlt

# 2.5 Linearisierung nicht-linearer Systeme
Beispiel: Mathematischs Pendel
dphi/dt= omega
domega/dt = -g/l.sin(phi)

dx/dt = f(x), x0  x=[phi, omega]^T
wR=0
sin(phiR)=0 folglich phiR1=0, phiR2=pi (hier gibt es eigendlich unendlich viele lösungen für phi, weil der R^2 verwendet wurde
                der R^2 ist der falsche Zustandsraum, der richtige Raum wäre eigendlich der SO3, der Zylinder?)

d[deltaphi, deltaomega]/dt^T=[[0, 1], [-g/l.cos(phiR), 0]].[deltaphi, deltaomega]^T

Ausgangslage (linearisierung um die untere Ruhelage):
    wR=0, phiR1=0
    Á=[[0, 1], [-g/l, 0]]
    det(A-lambda.I)=det[[-lambda, 1], [-g/l, -lambda]]=0
    lambda1,2=+-I.sqrt(g/l)  - Klassische Eigenwerte für einen ewig schwingendes, ungedämpftes System
        I=sqrt(-1)  um Verwechslungen mit Laufindices zu vermeiden

Ausgangslage (linearisierung um die obere Ruhelage)
    wR=0, phiR2=pi
    Á=[[0, 1], [g/l, 0]]
    det(A-lambda.I)=det[[-lambda, 1], [g/l, -lambda]]=0
    lambda1,2=+-sqrt(g/l)  - Klassische Eigenwerte für einen ewig schwingendes, ungedämpftes System
Linearisierung ist ein Werkzeug, das sehr systematisch und sehr einfach angewandt werden kann.
In so einem einfachen Fall, kann natürlich auch mit der "Kleine-Winkel"-Näherung linearisiert werden.
Doch dann muss auf den Winkel geachtet werden, um den linearisiert wird (Näherung nur bei phi=0 gültig).
Mit dieser Methode mit der Jakobimatrix liegt man jedoch immer am richtigen Weg.
    -Fazit: diese Methode (Linearisierung mittels Jakobimatrix) ist bombensicher

# linearisierung um die Trajektorie
Annahme: Eine Trajektorie eines Endeffektors wird idealisiert bestimmt. Was passiert, wenn Störungen
auf dem Pfad auftreten?

dx/dt=f(x,u), x0
y=h(x,u)

u~(t) folgt x~(t) folgt y~(t)
x(t) = x~+deltax
u(t) = u~#deltau
y(t) = y~+deltay

Taylorentwicklung
dx~/dt + ddeltax/dt = f(x~+dektax, u~+deltau)
                    ~= f(x~, u~) + pard/
analoges für die Ausgangsgröße
siehe Skriptum (Folie 95)
zwischennotiz: Im Anhang gibt es auch detailreiche Beweise (nicht Prüfungsstoff)

Beispiel: Rakete (zeitlich veränderliche Masse)
siehe Skriptum

Zusammenfassung:
    - was ist eine Ruhelage?
    - bei linearen Systemen gibt es entweder 0, 1, oder inf Ruhelagen
Nächste Stunde:
    - was für Systemverhalten können aus den Eigenwerten gelesen werden?
    - Tools: Jordan-Normalformen, Linearkombinationen, ...
Wir befinden uns nochimmer am besten Weg zum Regelkreis!
