# Your Project Name

| | |
|-|-|
|`Author` | Ciocan Vlad Stefan

## Description
Le projet consiste à concevoir un système de sécurité basé sur une carte Arduino Uno, capable de détecter la proximité d’un objet ou d’une personne à l’aide d’un capteur à ultrasons. Lorsque la distance mesurée devient inférieure à 15 cm, le système déclenche une alarme sonore et affiche un message d’avertissement « DO NOT TOUCH » sur un écran LCD. Le système reste en état d’alerte jusqu’à ce qu’un code PIN correct soit saisi à l’aide d’une télécommande infrarouge. Le récepteur IR permet de capter les signaux envoyés par la télécommande et de les interpréter afin de vérifier le code entré par l’utilisateur. En cas de code correct, l’alarme est désactivée et le système revient à son état initial de surveillance. En cas de code incorrect, l’alarme continue.

## Motivation
Ce projet a été choisi afin de démontrer la réalisation d’un système de sécurité simple mais efficace, en utilisant des technologies accessibles comme Arduino et des capteurs de proximité. La motivation principale est de comprendre comment combiner plusieurs composants matériels pour créer un système interactif capable de détecter des actions indésirables et de réagir en temps réel. L’intégration d’un mécanisme d’authentification via une télécommande infrarouge ajoute un niveau supplémentaire de complexité et de réalisme, en simulant des applications concrètes dans le domaine des systèmes d’alarme et du contrôle d’accès.

## Architecture
[Mode surveillance]
        |
        | distance < 15 cm
        ↓
[Mode alarme]
        |
        | saisie du PIN par télécommande
        ↓
[Validation du code]
   |              |
PIN correct   PIN incorrect
   ↓              ↓
Retour        Alarme maintenue
surveillance
### Block diagram

<!-- Make sure the path to the picture is correct -->
![Block Diagram](schematics/block_diagram.png)

### Schematic

![Schematic](schematics/kicad_schematic.png)

### Components


<!-- This is just an example, fill in with your actual components -->

| Device | Usage | Price |
|--------|--------|-------|
| Activ Buzzer | Buzzer | [1.5 RON](https://www.optimusdigital.ro/ro/audio-buzzere/635-buzzer-activ-de-3-v.html?search_query=buzzer&results=61) |
| Push Button | Button | [1 RON](https://www.optimusdigital.ro/ro/butoane-i-comutatoare/1119-buton-6x6x6.html?search_query=buton&results=222) |
| Jumper Wires | Connecting components | [7 RON](https://www.optimusdigital.ro/ro/fire-fire-mufate/884-set-fire-tata-tata-40p-10-cm.html?search_query=set+fire&results=110) |
| Breadboard | Project board | [10 RON](https://www.optimusdigital.ro/ro/prototipare-breadboard-uri/8-breadboard-830-points.html?search_query=breadboard&results=145) |

### Libraries

<!-- This is just an example, fill in the table with your actual components -->

| Library | Description | Usage |
|---------|-------------|-------|
| [lib-name1](link-to-lib) | official description of the lib | Used for accesing the peripherals of the microcontroller  |
| [lib-name2](link-to-lib) | official description of the lib | Used for accesing the peripherals of the microcontroller  |

## Log

<!-- write every week your progress here -->

### Week 6 - 12 May

### Week 7 - 19 May

### Week 20 - 26 May


## Reference links

<!-- Fill in with appropriate links and link titles -->

[Tutorial 1](https://www.youtube.com/watch?v=wdgULBpRoXk&t=1s&ab_channel=BenEater)

[Article 1](https://www.explainthatstuff.com/induction-motors.html)

[Link title](https://projecthub.arduino.cc/)
