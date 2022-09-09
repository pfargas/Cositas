# Descripció del videojoc

Món 3D en primera persona (millor interacció personatge-mapa) amb l'objectiu de passar de sala en sala per arribar al final del recorregut. Per fer això s'haura de superar una sèrie de reptes on hi haurà involucrats diversos efectes quàntics com, per exemple, l'efecte túnel o l'entrellaçament. Si es pot també es farà una sèrie de sales extres amb efectes relativistes.
Estarà pensat per un gran públic: s'exposaran tots els efectes quàntics abans de necessitar-se, amb una explicació rigorosa però entenedora i s'ensenyarà l'equació que segueix l'efecte descrit. Es recomana un nivell matemàtic de batxillerat, tot i que es podrà entendre qualitativament sense aquest requisit.

# Objectius
1. Desenvolupar un videojoc tipus puzzle on per avançar s'hagi d'aplicar un o varis efectes quàntics
2. Exposar els efectes quàntics més comuns i vistosos 
3. Càlcul numèric d'aquests efectes (com per exemple la resolució de l'equació de Schrödinger per aplicar l'efecte túnel)
## Estat actual
- S'està estudiant el funcionament de Unreal Engine 4, modelització 3d i programació en c++; junt amb un curs de mecànica quàntica per tal de fer el joc el més fidel possible a la realitat d'avui. 

_____________________________________________________________
## COSES PER FER

#### Fenomens a representar

- Efecte compton

  $\Delta \lambda = \frac{h}{m_e c}(1-\cos\theta)$
- Efecte fotoelectric

$E=h\nu-W_0$ where $W_0\equiv h \nu_0$ is the minimum energy required to remove an electron from the surface of the material.
- Efecte Tunel

$-\frac{h^2}{4\pi m} \dfrac{d^2}{dx^2} \psi(x)+V(x)\psi(x)=E\psi(x)$
- Principi d'incertesa de Heisenberg

$\sigma_x\sigma_p\geq \frac{h}{4\pi}$
- Entrellaçament

$\psi(x)=\frac{1}{\sqrt{2}}(|+->+|-+>)$
- DOBLE ESCLETXA I SUPERPOSICIÓ

$d\sin\theta\approx d\theta$
- Cos negre?

Use it to control the energy of some laser by changing the temperature of the source
- RELATIVITAT (ESPECIAL)

Really difficult to implement

### IDEES

- Començar per efecte fotoelèctric. Explicar el fenòmen extrany d'aquest efecte. Tenir-lo sempre present pero passar ràpid
- Explicar efecte Compton. Porta amb un sensor de color que detecti un color més baix que l'inicial. Discretitzar l'angle per no complicar els càlculs
- "Entrem al món quàntic" PRINCIPI D'INCERTESA: Explicar, petita prova i tenir present tota l'estona. Sobretot jugar amb posició moment, altres variables conjugades es poden esmentar pero crec que són molt més complicades de treballar amb elles
- Començar amb les coses rares: SUPERPOSICIÓ (gat de Schrödinger) Efecte túnel i entrellaçament com a principals
- Lo de relativitat ja veurem com es fa
- Jugar amb barreres de potencial i fer els problemes 1D al màxim

### PLAYSTYLE

- Menu circular amb els objectes necessaris: Mesurador de posició, moment, làser per augmentar E... (són exemples, no cal que fem aquests ni res)
###### Efecte túnel
- Potencial barrera quadrada (posem parets?). Es podria representar amb un "canó" de partícules que disparen a una paret (una paret tova, tal que la seva energia per traspassar V sigui V>E E=energia particula) i simular un detector a l'altra banda amb els càlculs de probabilitats correctes (estan fets als apunts de FQ)
- A nivells avançats, utilitzar la propietat de cos negre per canviar l'energia del làser.
- Es podria fer que el jugador mai afectés la mesura: no fos un observador quàntic. Així pots veure que passa sense afectar la mesura i és molt més fàcil el codi

________________________________________________________________________________________________________________________________________________

# Naming Convention
- SM_Rock_00 -> Static Mesh for rock version 00
- T_Rock_00_BC-> Base Colour Texture for rock version 00
- SKM_Rock_00 -> Skeletal Mesh for rock version 00
- T_Rock_00_N -> Normal map for rock version 00
- MAT_Rock_00 -> Material for rock version 00

REMEMBER TO NAME THE WORLD OUTLINER
