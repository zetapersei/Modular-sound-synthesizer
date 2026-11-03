# Sintetizzatore analogico modulare

Progetto di un sintetizzatore analogico modulare ispirato all'architettura dei
sintetizzatori classici, come quelli della tradizione Moog. Nasce da un mio
progetto personale a cui ho lavorato tra il 1978 e il 1980; gli schemi
conservano quell'idea e sono stati raccolti e ridisegnati in KiCad.

Il repository contiene la documentazione elettronica del progetto: uno schema
principale gerarchico, gli schemi dei singoli moduli, un progetto PCB e il
netlist. Non contiene firmware o software per generare il suono.

## Moduli

| Modulo | Funzione |
| --- | --- |
| **VCO** | Oscillatore controllato in tensione: genera il segnale di base. |
| **VCF** | Filtro controllato in tensione, indicato nello schema come filtro PAiA 4730. |
| **VCA** | Amplificatore controllato in tensione: regola il livello del segnale. |
| **ADSR** | Generatore d'inviluppo per articolare nel tempo il suono. |
| **LFO** | Oscillatore a bassa frequenza per modulazioni lente. |
| **Generatore di rumore** | Sorgente di rumore per ulteriori timbri e modulazioni. |
| **Mixer audio** | Somma le sorgenti audio. |
| **Encoder per tastiera** | Schema per l'interfaccia di una tastiera musicale a 49 tasti. |

I moduli sono organizzati nello schema principale [`analog_synth.kicad_sch`](analog_synth.kicad_sch);
ogni circuito ha anche il proprio schema separato. I nomi dei file dei moduli
corrispondono alle sigle riportate nella tabella.

## Aprire il progetto

Apri [`analog_synth.kicad_pro`](analog_synth.kicad_pro) con KiCad per accedere
al progetto, allo schema gerarchico e al PCB [`analog_synth.kicad_pcb`](analog_synth.kicad_pcb).
È possibile aprire direttamente anche il file dello schema principale.

## Stato del progetto

Gli schemi documentano l'architettura e i circuiti, ma il repository non
specifica lo stato di realizzazione o collaudo dell'hardware. Prima di
costruire o alimentare i circuiti, verifica schemi, netlist, footprint,
componenti e tensioni richieste.

## Licenza

Il progetto è distribuito secondo i termini della licenza GNU GPL versione 3;
consulta [`LICENSE`](LICENSE) per il testo completo.
