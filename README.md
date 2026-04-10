# Artificial-pancreas

## Opis
Projekat analizira sistem veštačkog pankreasa koji automatski reguliše nivo glukoze u krvi pomoću zatvorene upravljačke petlje.

## Princip rada
1. Merenje glukoze  
2. Izračunavanje greške  
3. Određivanje doze insulina  
4. Ubrizgavanje insulina  
5. Povratna sprega   

## Minimalni model
dG/dt = -(SG + x)G + C  
dx/dt = kaI - kb x  

Radna tačka: (7.5, 0.009, 15)

## Linearizovan model
dx1/dt = -0.023x1 - 7.5x2  
dx2/dt = 6·10^-6 u - 0.01x2  

## Regulator
Koristi se PID regulator:  
Gr(s) = kd s² + kp s + ki  

Parametri:  
Kd = -711  
Kp = -24.9  
Ki = -0.2  

## Stabilnost
Sistem je stabilan (Nyquist analiza).  

