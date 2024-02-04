# Cinematismi
### Opzione 1: avendo i vincoli di assieme
(ricorda di fissare uno degli oggetti)

- spostarsi nell'ambiente DMU Kinematics
- **Assembly constraint conversion** (due ruote dentate)
    - New mechanism
    - Auto create (per creare i cinematismi in automatico)
- editare i giunti per fissarne i range (solo per sim con comando)
    - lenght driven
    - si può fare tasto destro > measure between per misurare una distanza
- CATIA mostra un avviso: "The mechanism can be simulated"
    - accanto al nome del meccanismo è indicato il numero di DOF


### Opzione 2: senza vincoli di assieme
- creare un giunto di tipo **fixed part** per fissare una parte
- aggiungere un **rigid joint** tra le coppie di oggetti fissati
- **prismatic joint**: servono una linea e un piano comuni tra le due parti


## Simulazioni

### Generazione delle simulazione via comandi
Simulation with Commands

Per attivare i sensori, spuntare _Activate sensors_


### Generazione delle simulazione via legge oraria
- aprire il command interessato
- command value > click dx > edit formula
- nella legge oraria, il tempo è un parametro che si trova sotto Time
- _Simulation with Laws_
- scegliendo un valore appropriato di secondi di simulazione e sfruttando il plotting dei sensori si può ottenere il grafico spazio-tempo

Leggi orarie:

> velocità:  
> Lunghezza=10mm/1s*Meccanismo.1\KINTime  
> accelerazione:  
> Lunghezza=10mm/1s* Meccanismo.1\KINTime+0.5*2mm/1s*1s*Meccanismo.1\KINTime*Meccanismo.1\KINTime 







