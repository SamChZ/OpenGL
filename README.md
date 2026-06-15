# Workshop 2 – Terrain Renderer

Gemaakt voor Computer Graphics Workshop 2. Het laadt een heightmap in en tekent daar een 3D terrein mee, met shaders voor verlichting en kleur. Gebouwd met C++, OpenGL, SDL en GLEW.

## Bouwen en uitvoeren

```bash
make
./workshop2
```

Werkt op Linux (getest op Ubuntu / room 302 / titan). Je hebt SDL 1.x, GLEW en OpenGL nodig.

## Wat er in zit

De belangrijkste onderdelen zijn de geometry klassen (Vector2, Vector3, Vector4, Matrix4), een SDL wrapper die het venster en de input afhandelt, en een shader loader die de vertex- en fragmentshaders inlaadt tijdens runtime. De heightmap (`heightmap.raw`) is een 513×513 8-bit grayscale bestand.

## Even weten

- Het terrein is op dit moment vlak — de hoogtemap wordt wel ingeladen maar de z-waarde van de vertices wordt nog niet gebruikt. Dat was een onderdeel voor tijdens de workshop zelf.
- Camerabesturing via het toetsenbord is ook nog niet geïmplementeerd.
- Afsluiten doe je met Escape of het kruisje.
