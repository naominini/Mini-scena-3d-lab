# Sistem Solar 3D

Scenă 3D interactivă a sistemului solar realizată cu **Three.js** (WebGL)

## Tehnologii utilizate

- **Three.js r128** — engine 3D bazat pe WebGL pentru randare, geometrii, materiale și lumini
- **OrbitControls** — navigare cameră interactivă (rotire, zoom, pan cu mouse)
- **BufferGeometry** — geometrie optimizată pentru centura de asteroizi și coada cometei
- **MeshStandardMaterial** — materiale cu iluminare fizică realistă (PBR) și texturi 2K
- **MeshBasicMaterial** — materiale fără iluminare pentru Soare, glow și skybox
- **PointsMaterial** — sistem de particule pentru asteroizi și coada cometei
- **HTML5 / CSS3** — interfață UI cu panou lateral animat (slide + backdrop blur)
- **ES Modules + Import Maps** — import Three.js direct din CDN fără bundler

## Funcționalități

- 8 planete cu texturi 2K, orbite vizibile, rotație proprie și viteze diferite
- Luna care orbitează Pământul (pivot nested)
- Inele Saturn cu UV mapping personalizat și transparență
- Efect de glow atmosferic colorat în jurul planetelor
- Centura de asteroizi animată între Marte și Jupiter
- Cometă cu coadă de particule multi-strat (efect fade)
- Skybox Milky Way 360° pe sferă interioară
- Iluminare realistă de la Soare (PointLight) + lumină ambientală
- Panou lateral cu focus smooth pe fiecare planetă (lerp)
- Cameră cu FOV wide și OrbitControls cu damping

## Cum se rulează

Proiectul folosește ES Modules și texturi locale, deci **nu funcționează dacă deschizi fișierul direct** (dublu click).

1. Instalează extensia **Live Server** în Visual Studio Code
2. Click dreapta pe `scena3d.html` → **Open with Live Server**
3. Se deschide automat în browser la `http://127.0.0.1:5500/scena3d.html`

## Surse texturi

[solarsystemscope.com](https://www.solarsystemscope.com/textures/)