# KayakVR-HTC
Unity PCVR software that simulates a kayak, for use in research.

**Manuscript ID:** IEEE LATAM Submission ID: 10516

**Authors** 
- Jorge Gonzáles-Ortega (1)
- Agustín Venegas (2)
- Ismael Gallardo (2)
- Felipe Besoaín (1)

**Affiliation**

1. Department of Interactive Visualization and Virtual Reality, Faculty of Engineering, Universidad de Talca
2. Faculty of Psychology, Universidad de Talca

## Included Scripts and Assets
This repository contains all scripts and assets required to build and run the simulation and obtain the results presented in the article.

| Script | Description |
|--------|------------------|
| KayakController.cs | Main script of the simulated kayak. Applies forces according to parameters of speed and torque, when the paddle is moved underwater. |
| Paddle.cs | Simulates each blade of the paddle. Calls functions on the KayakController script when the paddle object is moved underwater. |
| BuoySequence.cs | A ScriptableObject class that stores data of the messages (texts, and images) shown to users during gameplay. |
| BuoyManager.cs | Manages the in-game buoys, and shows message panels to users according to the BuoySequence used. |
| MainBuoyEditorWindow.cs | An editor window script. It is used to edit BuoySequence objects, adding, changing or rearranging the messages. |
| LogManager.cs | Object that stores the actions of interest performed by the users (ex. time until they reached the first buoy). It also writes a .csv file with the data after the game ends. |
| LogEvent.cs | Saves a string (ex. "EnteredBuoy1") and the time since the program started, in seconds, when called. LogManager then retrieves this string. |

## Requirements
Requires a VR Ready, Windows PC.
Unity 2021 LTS, latest version.
SteamVR configured as XR Loader.

## Contact
For questions or replication of results:
avenegas19@alumnos.utalca.cl
