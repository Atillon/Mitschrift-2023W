# Einleitung

Vorlesung bringt den Inhalt
Videos bringen die Vertiefung, extreme Details in den Videos

Prüfungsmodus:
Handschriftlich + Formelzettel
Erste Prüfung: Mitte-Ende Februar

# Was ist Photonik

Ein wenig Geschichte:
-) Nobelpreise

Ein wenig wirtschaftliche Relevanz

Modelle der Photonik:
-) Quantenelejtridynamik
-) Naxwellsche Elektrodynamik
-) Geometrische Optik

# Kapitel 1?
nablaxE=-dB/dt ,   nablaxH=dD/dt + J
D=e_0.E+P, P=e_0.ksi.E, ksi=ksi(w)
nabla.nabla.1/c_0^2.d^2E/dt^2 = µ_0.d^2P/dt^2
Wir sehen, beschleunigte Ladung strahlt Photonen (Energie) ab.
Links:Ausbreitungsterm, Rechts: Quellterm
Weiters: e_r=1+ksi oder n=sqrt(e_r), in der Photonik wird eher der Brechungsindex statt ksi verwendet.
nabla^2.E-n^2/c_0^2.d^2E/dt^2=0

E=Re{E_ampl*e^(jwt)}=1/2*(E_ampl.e^(jwt) + kk-Anteil}
Eingesetzt:
[nabla^2-n^2/c_o^2(-w^2)]E(w)=0

E(w)=E_0.e^(jkx)
Eingesetzt:
(-jk)(-jk)+n^2/c_0^2w^2]E(w,k)=0
-k^2+n^2/c_0^2.w^2=0  daraus folft k(w) =w/c_0.n(w) ...Dispersionsgleichung
aus der Dispersionsrelation kann der Impuls eines Wellentyps bestimmt werden. In diesem Fall ist p=h_quer.k(w)=linear im Vakuum

Beziehung bei ebenen Wellen

E=E_0.e^j(wt-kx)
nablaxE=-µ0dH/dt
-jkxE-µojwH
H0kxE/µ0w

H=k/µ0w.E, k=w/c0.n

H=n/2z0.E, z0=sqrt(µ0/e0)

E=E0cos(wt-kx)
kx=kz
cos(-ks)=1
ks=m2pi
deltaz=2pi/k=lambda
k=2pi/lambda

Wir suchen die Ausbreitungsgeschwindidkeit
Extrema der Welle ableiten
d/dt(wt-kz)=d/dtm2pi
w-dz/dt=0
vP=w/k=c0/n, lambda =2pi/k
vp =w/(2pi/lambda)=lambda.w/2pi=lambdaf=c0/n

S=ExH=K/2µ0w.BetragE ^2=n/2z0betragE^2=I ... Intensität
P=integral über A von I nach DA

Polarisation
Skizze von E-Vektor in der  x-y Ebene

E=(Ex.ej(wt-kz) Ey.e^j(wt-kz))^T ...linear polarisiert
E=(Ex.ej(wt-kz) Ey.e^j(wt-kz)+-pi/2)^T ...zirkular polarisiert
rechts oder links zirkluar ist abhängig von der Definition aber die Physiker gehen nach der rechtschraube

E=(Ex.ej(wt-kz) Ey.e^j(wt-kz)+-jpi/2)^T   ...elliptisch zirkular

wenn die Phasenverschiebung nicht pi/2 ist (zB pi/8) ist es weiterhin elliptisch zirkular, aber im Raum verdreht (siehe detailierte Herleitung in den Videos)

# Jones Vektor 
J = ( Ex Ey.ejdeltay)^T
(Ex1 Ex2 e^jwt)^T=(a b ,c d)(Ex Ey.e^jwt)^T


Do. 12.10.2023
 Vergessen zu speichern, hier fehlt einiges.
Wiederholung: Helmholtzgleichung ist nichts anderes als Wellengleichung wo sinusförmiges Signal iengesetzt wurde

E=E0.e^j(wt-kz) H=kxE/µ0w (das gibt uns ein Dreibein - rechtwinkeliges Koordinatensystem)

Herleitung Snellius-Gesetz (Brechungsgesetzt): siehe Foto

Ei + Er = Et
(Ei.e^j(wt-kiz))'' + (Er.e^j(wt-krz))'' = (Et.e^j(wt-ktz))''           ()'' ... Tangentialkomponente ?

ki'' = kr'' = kr''

kisin(thetai)  = kr . sin(thetar) = kt.sin(thetat)
k0.ni.sin(thetai) = k0.nr.sin(thetar)=k0.nt.sin(thetat)  ... Reflexionsgesetz

Skizze (siehe Foto)

# Fresnel'sche Gleichungen
Propargant der Wellentheorie im Kampf gegen die Korpuskeltheorie.
Wir haben wieder die einfallende Welle vom vorherigen Beispiel. (siehe weiters Skizze zu Fresnel Koeffizienten)

Einfallende Welle Ei^sp = t^sp.Ei           E,,^i + E,,^r =E,,^t
Reflektierte Welle Er^sp = r^sp.Ei          H,,^i + H,,^r = E,,^t
                                            kxE/µ0w=H
        siehe Skript für alle Fresnelt-Koeffizienten
        Fresnel-Koeffizienten brauchen nicht auswendig gelernt werden.

Pi = Pr + Pt ... Leistungserhaltung
Leistung ist Intensität mal Fläche. Leider reicht I = n Betrag(E)^2 / 2z0 aus
letzter VO nicht aus, weil die Flächenprojektion berücksichtigt werden muss.
Sonderfall: Fleicher Einfalls- wie Ausfallswinkel
        siehe Skizze(Foto) für Abbildung der flächen
        At = pi.bz.at
        P = i.A
        Pi = Pr + Pt
        Ii . Ai = It.Ar + It.At
        niBetrag(Er)^2 / 2z0 . Ai = niBetrag(Er)^2 / 2z0 . Ar + nt.Betrag(Et)^2 / 2z0 . At
        Er=rEi
        Et=tEi
        ni.Betrag(Ei)^2.Ai = ni.Betrag(r)^2Betrag(Ei)^2.Ai + nt.Betrag(t)^2. Betrag(Ei)^2.At
        1 = Betrag(r)^2 + nt/ni . Betrag(t)^2 . At/Ai
        1 = Betrag(r)^2 + Betrag(t)^2.nt/ni.costhetat/costhetai
        1 =    R        +      T = Reflektivität + Transmitivität

wichtiges Bild:
    x-y plot R von theta_i: [0°; 90°]
    R^s ~=0.04 . exp(theta_i)
    R^p ~= 0.04 .exp(theta_i) + Tal bei theta B (theta B brewsterwinkel, hier ist die Reflektivität der parallelstrahlung 0)
    Beim brusterwinkel ist der Winkel zwischen reflektiertem und transmit
    -tiertem Strahl exakt 90°. Das polarisierte Licht erzeugt ja Dipole in der
    Materie. Diese Dipole senden bekanntlich wieder Licht aus. Diese Hantel
    -förmigen (cos^2-förmigen) Dipole strahlen in Querrichtung ab und das sorgt
    irgendwie dafür, dass es da kein R^p gibt.
    thetaR+thetat+90°=180°
    ni.sin(thetai)=nt.sin(thetat)
    ni.sin(thetai)=nt.sin(90-thetai)
                    ^^^^^^^^^^^^^^^
                        COS(THETA_I)
    tan(thetai)=nt/ni
    thataB = arctan nt/ni       Beispiel, nt=1,5, ni = 1 daraus folgt thetaB = arctan1,5 = 56°

Warum gibt es trotzdem Reflektivität für s-polarisiertes Licht?
        Hab ich nicht gehört, also überlegs dir selbst!
Die Sonnenstrahlung ist nicht gefiltert, hat somit alle Polarisationen. Die
Reflektion am Boden ist aber Hauptsächlich s-polarisiert, da r-polarisiert
immer viel schwächer ist. Deshalb kann man das s-polarisierte gezielt mit
polarisierten Gläsern filtern.

Es folgen einige geometrische Beispiel welche uns letztendlich zur Total
-reflexion führen. Die Wellenvektoren werden betragsmäßig als Halbkreise vom
Auftrittspunkt aus gezeichnet. Dadurch können mithilfe der Winkel einige
geometrische Griffe durchgeführt werden.

Wenn der Radius der Reflexion größer ist, als der der Transmission, gibt es
einen kritischen Winkel theta_c, ab dem keine Lösung mehr existiert.
k_n^2 + k,,^2 = kt^2              k,, ... k parallel, kn .... k normal
kn = sqrt(kt^2-k,,^2)
kn = +- sqrt(kt^2 - (ki.sin(thetai))^2)    nt kleiner ni
kn = +- k0 sqrt(nt^2-(ni.sin(thetai)^2))
kn = +- kojsqrt(nr.sin(thetai)^2-nt^2)=+-jgamma     thetai größer theta r
Et = E0.e^(wt - kn.z -k,,.x)
Et=E0.e^-+gamma.z.e^j(wt-k,,.x)
        ^^
        muss '-' sein, weil es exponentiell fallen muss
        (physikalisch richtige Interpretation)
Man nennt dieses exponentiell fallendes Feld ein evaneszentes Feld.
Eine Anwendung für so ein evaneszentes Feld wird noch genau erklärt.

Man betrachte wieder das Einfallsdiagram:
    Wenn der Radius der Reflexion größer als der Radius der
    Transmission ist, liegt der kritische Winkel bei 90°.
    Mathematische Herleitung für den kritischen Winkel:
        ni.sin(thetac) = nt.sin(thetat)
        theta_c=arcsin(nt/ni)
        theta_c=arcsin(1/1,5)=41,8
