# 🔮🗡️⚔️🏹✝️ La Ascensión Del Heroe 🏰

Un juego de rol por turnos basado en consola donde el jugador crea y gestiona héroes que ascienden por la temida **La Ascensión Del Heroe**. Usa estrategia, equipo y habilidades únicas para sobrevivir a enemigos cada vez más peligrosos. ¡Una experiencia narrativa, efectos temporales y progresión por niveles!, Administratas tu equipo, mejoraras tus habilidades, te especializaras en una categoria. 

---
---
## Historia y Narrativa:

En el reino de *O'Dromos* Su gobernante y su mesa de 5 consejeros pensando en la manera de tener un gran heroe poderoso y valiente idean usar sus habilidades, conocimientos y experiencias para crear una Torre, donde todos los heroes del Reino puedan adentranse y acender para obtener el titulo de guardian del reino, junto con ellos reputacion, dinero, fama y gloria, diseñaros este desafio para ser cada nivel mas dificol que el anterior y asi solo el Heroe que realmente lo merezaca pueda hacerte con la recompenza.

### Notas:

- La narrativa sera una parte central de el juego ya que esta busca integrar historias entre niveles, algunas para enemigos o aliados.
- La histora podria tener varios finaes correspondiente a las deciciones tomadas durante el juego

---

## 🛠️ Tecnologias

- Node.js
- JavaScript
- MongoDB
- Librerias npm

---

## 🎮 Características Principales

- ✅ Creación de personajes con clases únicas: **Guerrero**, **Mago**, **Arquero**, **Asesino** y **Sacerdote**
- ⚙️ Mecanicas de especializacion de clases 2 por cada una con sus propias habilidades, (pergaminos) como recompenza por nivel para potencias habilidades de su especializacion
- 📊 Sistemma de estaditicas como: 
            **Aguante**-> Modifica la salud maxima, 
            **Fuerza** -> Potencia las habilidades de daño fisicas del Guerrero, 
            **Agilidad** -> Potenica las habilidades del cazador y el Asesino,
            **Inteligencia** -> Potenica las habilidades magicas del Mago,
            **Sabiduria** -> Potenica las habilidades sagradas del Sacedote,
- 📝 Las estadisticas seran base de 10 para todos los persoanjes pero al se les daran 20 puntos para distribuir como quiera y asi potenciar segun lo que aplique a su estrategia
- 🧩 Sistema de inventario dinámico: armas, armaduras, pociones y objetos especiales.
- ⚔️ Combate por turnos con habilidades y decisiones tácticas.
- 🧠 IA básica de enemigos.
- 🏆 Subida de nivel por experiencia y progresión tras cada batalla.
- 🌈 Interfaz visual en consola.
- 💾 Guardado persistente en formato JSON.
- 🔁 Repetición de combates, gestión de personajes y personalización posterior.
- ☠️ De inicial el juego estara planteado con una dinamica de que al perder el persoanje se borrara y tendras que crear uno nuevo
- 💰 Implmentar un sistema de monedas de Acension las cualse se canjearan en tiendas que estaran cada 3 niveles de la torre
- 🏅 Sistema de niveles y especializacion cada clase tendra 2 especializaciones y mejoras las cuales se aplicaran en cada nivel segun eleccion del jugador.

---

## 🧠 Mecánicas del Juego

### 👤 Clases Jugables

| Clase         | Descripción                                                                           |
|---------------|---------------------------------------------------------------------------------------|
| 🛡️ Guerrero   | Especialista en defensa física, usa armas pesadas y escudos.              
| 🏹 Arquero   | Experto en ataques a distancia y trampas                                 
| 🔮 Mago      | Poder ofensivo mágico de fuego hielo o manejo de artes arcanas           
| 🗡️ Asesino   | Combatiente Sigiloso aprovechando la oscuridad y la sorpresa                         
| ✝️ Sacerdote | Experto en el manejo de la luz ya sea castigando a con luz segadora o absorbiendo daño   

Cada clase tiene acceso a habilidades únicas según su rol y especializacion

---

### 🧰 Sistema de Inventario

- Maneja un inventario limitado por manos para las armas y equipamientos.
- Equipamiento activo afecta estadísticas del personaje.
- Uso de **pociones** y **cambio de objetos** en combate.
- Objetos tienen modificadores como:
  - para habilidades especificas segun clase y especializacion.

---

### ⚔️ Combate y Habilidades

- Sistema **por turnos** con IA de enemigos.
- Habilidades definidas en cada clase
- Menú interactivo para usar habilidades o gestionar el inventario.
- Al finalizar combate:
  - El personaje Gana de experiencia
  - Puede obtener mejoras o nuevos objetos (por implementar).
  - Si muere, su progreso se pierde y se elimina hasta el ultimo nivel con un guardado.

---

### 📦 Guardado y Base de Datos

- El juego guarda automáticamente los personajes en archivos en formato JSON locales de forma temporal durante el juego.
- La base de datos de Personajes guardados, progrecion, armas, armaduras, objetos, enemigos y demas se guardaran de forma remota con MongoBD.

## 🏗️ Estructura del Proyecto

```
La Ascension Del Heroe/
├── src/                            # Estrcuturacion de codigo clave
|   ├── data/                       # Archivos JSON temporales
│   |   ├──                         # 
│   |   ├──                         # 
│   |   └──                         # 
|   ├── bd/                         # Conexión MongoDB y lógica de persistencia
│   |   ├──                         # 
│   |   ├──                         # 
│   |   └──                         # 
│   ├── models/                     # Sistema de herencia de clases
│   │   ├──                         # 
│   │   └──                         # 
│   ├── services/                   # Lógica de negocio (combate, inventario, etc.)
│   │   ├──                         # 
│   │   └──                         # 
│   ├── ui/                         # Interacciones CLI con el jugador
│   │   ├──                         # 
│   │   └──                         # 
│   └── utils/                      # Helpers y utilidades generales
│       ├──                         # 
│       └──                         # 
├── .gitignore                      # Archivos ignorados por Git
├── index.js                        # Punto de entrada principal
├── package.json                    # Librerias instalas y versiones de las mismas
├── package-lock.json               # Configuracion de NODE
└── README.md                       # Descripcion del proyecto
```
---

## 📥 Instalación

```bash
git clone https://github.com/Brian-s47/Simulador-de-Batallas-RPG.git
cd Simulador-de-Batallas-RPG
npm install
```

---

## 🚀 Ejecutar el Juego

```bash
node index.js
```

---

## 🛠️ Tegnologias Usadas

- Node.js
- JavaScript
- MongoDB
- Librerias npm

---

## 🧑‍🤝‍🧑 Créditos

> Desarrollado por:

- **Brian Fair Suarez Porras**

