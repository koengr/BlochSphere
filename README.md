# BlochSphere
Mathematica functions that plot time-evolution on a Bloch Sphere.

Some example functions require the MaTeX package:
https://github.com/szhorvat/MaTeX

Many essential parts were taken from StackOverflow user glS:
https://mathematica.stackexchange.com/questions/125985/how-to-draw-an-interactive-mouse-clickable-3d-bloch-sphere


```Mathematica
energyGap = 9.3;
angularVelocity = 9;
resolution = 300;

hamiltonian = energyGap * Z / 2 + Cos[ angularVelocity t ] X;
initialstate = {1, 0};

EvolutionOnBlochSphere[ hamiltonian , initialstate,  {t, 0, 
  1.1 Pi  }, resolution ]
```

![Example of Bloch Sphere output](https://raw.githubusercontent.com/username/projectname/branch/path/to/img.png)

