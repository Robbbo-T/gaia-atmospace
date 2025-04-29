## GenAI Proposal Status Disclaimer

*Este documento es un análisis generado por GenAI y no ha sido validado por expertos en el dominio. Los detalles de implementación son teóricos y necesitarían revisión formal y validación por especialistas en ingeniería aeroespacial, astronáutica, tecnologías sostenibles e integración de IA.*

## 1. Overview

Este documento proporciona la estructura de directorios completa para el ecosistema GAIA PLATFORMS, con un enfoque particular en la implementación de la convención de códigos COAFI. La estructura está organizada en divisiones principales, cada una conteniendo módulos especializados que abordan aspectos específicos de tecnologías aeroespaciales, astronáuticas y sostenibles.

## 2. COAFI Code Convention

### 2.1 Purpose

La convención de códigos COAFI (Component-Organization-Application-Function-Identifier) proporciona una forma estandarizada de identificar y referenciar componentes dentro del ecosistema GAIA PLATFORMS. Esta convención asegura trazabilidad, consistencia y claridad en todo el proyecto.

### 2.2 Format

El formato general para los códigos COAFI es:

```plaintext
COAFI-[DIVISION]-[CLASS]-[COMPONENT]-[NUMBER]-[TYPE]
```

Donde:

- **DIVISION**: El código de división principal (ej., GPAM para GP-AM)
- **CLASS**: El identificador de clase (ej., 0100 para AMPEL)
- **COMPONENT**: Un código de 3 letras que representa el componente
- **NUMBER**: El número de capítulo ATA/AS
- **TYPE**: La inicial del modelo tecnológico (ej., GPA para General Platform Architecture)


### 2.3 Example

```plaintext
COAFI-GPAM-0100-ENG-72-GPA
```

Este código identifica:

- División: GP-AM (Aircraft Models)
- Clase: 0100 (plataforma AMPEL)
- Componente: ENG (Engine)
- Número: 72 (capítulo ATA para Engine)
- Tipo: GPA (General Platform Architecture)


## 3. Root Structure

```plaintext
GAIA-PLATFORMS/                                 # [COAFI-ROOT-0000-GPF-00-GPF](#coafi-root-0000-gpf-00-gpf) (Directorio raíz del ecosistema GAIA)
├── README.md
│
├── GAIA-AIRs/                                  # [COAFI-GAIR-0000-AIR-00-GPF](#coafi-gair-0000-air-00-gpf) (Plataformas aéreas y aeronáuticas)
├── GAIA-SPACEs/                                # [COAFI-GSPC-0000-SPC-00-GPF](#coafi-gspc-0000-spc-00-gpf) (Plataformas espaciales y astronáuticas)
├── GAIA-GROUND/                                # [COAFI-GGND-0000-GND-00-GPF](#coafi-ggnd-0000-gnd-00-gpf) (Infraestructura terrestre y aeroportuaria)
├── GAIA-GREEN-TECHNOLOGIES/                    # [COAFI-GGRN-0000-GRN-00-GPF](#coafi-ggrn-0000-grn-00-gpf) (Tecnologías sostenibles y ecológicas)
├── SharedServices/                             # [COAFI-SSRV-0000-SRV-00-GPF](#coafi-ssrv-0000-srv-00-gpf) (Servicios compartidos entre plataformas)
└── GP-FD/                                      # [COAFI-GPFD-0000-FND-00-GPF](#coafi-gpfd-0000-fnd-00-gpf) (Fundamentos y principios arquitectónicos)
```

## 4. GAIA-AIRs Structure

```plaintext
GAIA-AIRs/                                      # [COAFI-GAIR-0000-AIR-00-GPF](#coafi-gair-0000-air-00-gpf) (Plataformas aéreas y aeronáuticas)
├── README.md
├── AToC.md                                     # [COAFI-GAIR-0000-TOC-00-GPF](#coafi-gair-0000-toc-00-gpf) (Tabla de contenidos arquitectónica)
│
├── GP-AM/                                      # [COAFI-GPAM-0000-AIR-00-GPA](#coafi-gpam-0000-air-00-gpa) (Modelos de aeronaves)
│   ├── README.md
│   ├── AMPEL/                                  # [COAFI-GPAM-0100-AMP-00-GPA](#coafi-gpam-0100-amp-00-gpa) (Plataforma de modelado de aeronaves)
│   │   ├── ATA-00-GEN/                         # [COAFI-GPAM-0100-GEN-00-GPA](#coafi-gpam-0100-gen-00-gpa) (Información general)
│   │   ├── ATA-01-AMT/                         # [COAFI-GPAM-0100-AMT-01-GPA](#coafi-gpam-0100-amt-01-gpa) (Límites de tiempo de aeronave)
│   │   ├── ATA-02-OPS/                         # [COAFI-GPAM-0100-OPS-02-GPA](#coafi-gpam-0100-ops-02-gpa) (Operaciones)
│   │   ├── ATA-03-PERF/                        # [COAFI-GPAM-0100-PER-03-GPA](#coafi-gpam-0100-per-03-gpa) (Rendimiento)
│   │   ├── ATA-04-AIRW/                        # [COAFI-GPAM-0100-AIR-04-GPA](#coafi-gpam-0100-air-04-gpa) (Aeronavegabilidad)
│   │   ├── ATA-05-MAINT/                       # [COAFI-GPAM-0100-MNT-05-GPA](#coafi-gpam-0100-mnt-05-gpa) (Mantenimiento programado)
│   │   ├── ATA-06-DIM/                         # [COAFI-GPAM-0100-DIM-06-GPA](#coafi-gpam-0100-dim-06-gpa) (Dimensiones y áreas)
│   │   ├── ATA-07-LIFT/                        # [COAFI-GPAM-0100-LFT-07-GPA](#coafi-gpam-0100-lft-07-gpa) (Elevación y apuntalamiento)
│   │   ├── ATA-08-LEV/                         # [COAFI-GPAM-0100-LEV-08-GPA](#coafi-gpam-0100-lev-08-gpa) (Nivelación y pesaje)
│   │   ├── ATA-09-TOW/                         # [COAFI-GPAM-0100-TOW-09-GPA](#coafi-gpam-0100-tow-09-gpa) (Remolque y rodaje)
│   │   ├── ATA-10-PARK/                        # [COAFI-GPAM-0100-PRK-10-GPA](#coafi-gpam-0100-prk-10-gpa) (Estacionamiento y anclaje)
│   │   ├── ATA-11-PLAC/                        # [COAFI-GPAM-0100-PLC-11-GPA](#coafi-gpam-0100-plc-11-gpa) (Placas y marcas)
│   │   ├── ATA-12-SERV/                        # [COAFI-GPAM-0100-SRV-12-GPA](#coafi-gpam-0100-srv-12-gpa) (Servicio)
│   │   ├── ATA-13-HYD/                         # [COAFI-GPAM-0100-HYD-13-GPA](#coafi-gpam-0100-hyd-13-gpa) (Hidráulica)
│   │   ├── ATA-14-PNEU/                        # [COAFI-GPAM-0100-PNU-14-GPA](#coafi-gpam-0100-pnu-14-gpa) (Neumática)
│   │   ├── ATA-18-VIB/                         # [COAFI-GPAM-0100-VIB-18-GPA](#coafi-gpam-0100-vib-18-gpa) (Análisis de vibración)
│   │   ├── ATA-20-STD/                         # [COAFI-GPAM-0100-STD-20-GPA](#coafi-gpam-0100-std-20-gpa) (Prácticas estándar - Estructura)
│   │   ├── ATA-21-ECS/                         # [COAFI-GPAM-0100-ECS-21-GPA](#coafi-gpam-0100-ecs-21-gpa) (Control ambiental)
│   │   ├── ATA-22-AUTO/                        # [COAFI-GPAM-0100-AUT-22-GPA](#coafi-gpam-0100-aut-22-gpa) (Piloto automático)
│   │   ├── ATA-23-COMM/                        # [COAFI-GPAM-0100-COM-23-GPA](#coafi-gpam-0100-com-23-gpa) (Comunicaciones)
│   │   ├── ATA-24-ELEC/                        # [COAFI-GPAM-0100-ELC-24-GPA](#coafi-gpam-0100-elc-24-gpa) (Energía eléctrica)
│   │   ├── ATA-25-EQUIP/                       # [COAFI-GPAM-0100-EQP-25-GPA](#coafi-gpam-0100-eqp-25-gpa) (Equipamiento/Mobiliario)
│   │   ├── ATA-26-FIRE/                        # [COAFI-GPAM-0100-FIR-26-GPA](#coafi-gpam-0100-fir-26-gpa) (Protección contra incendios)
│   │   ├── ATA-27-FCS/                         # [COAFI-GPAM-0100-FCS-27-GPA](#coafi-gpam-0100-fcs-27-gpa) (Controles de vuelo)
│   │   ├── ATA-28-FUEL/                        # [COAFI-GPAM-0100-FUL-28-GPA](#coafi-gpam-0100-ful-28-gpa) (Combustible)
│   │   ├── ATA-29-HYD/                         # [COAFI-GPAM-0100-HYD-29-GPA](#coafi-gpam-0100-hyd-29-gpa) (Potencia hidráulica)
│   │   ├── ATA-30-ICE/                         # [COAFI-GPAM-0100-ICE-30-GPA](#coafi-gpam-0100-ice-30-gpa) (Protección contra hielo y lluvia)
│   │   ├── ATA-31-IND/                         # [COAFI-GPAM-0100-IND-31-GPA](#coafi-gpam-0100-ind-31-gpa) (Sistemas de indicación/registro)
│   │   ├── ATA-32-LG/                          # [COAFI-GPAM-0100-LND-32-GPA](#coafi-gpam-0100-lnd-32-gpa) (Tren de aterrizaje)
│   │   ├── ATA-33-LIGHT/                       # [COAFI-GPAM-0100-LGT-33-GPA](#coafi-gpam-0100-lgt-33-gpa) (Luces)
│   │   ├── ATA-34-NAV/                         # [COAFI-GPAM-0100-NAV-34-GPA](#coafi-gpam-0100-nav-34-gpa) (Navegación)
│   │   ├── ATA-35-OXY/                         # [COAFI-GPAM-0100-OXY-35-GPA](#coafi-gpam-0100-oxy-35-gpa) (Oxígeno)
│   │   ├── ATA-36-PNEU/                        # [COAFI-GPAM-0100-PNU-36-GPA](#coafi-gpam-0100-pnu-36-gpa) (Neumática)
│   │   ├── ATA-37-VAC/                         # [COAFI-GPAM-0100-VAC-37-GPA](#coafi-gpam-0100-vac-37-gpa) (Vacío)
│   │   ├── ATA-38-WATER/                       # [COAFI-GPAM-0100-WTR-38-GPA](#coafi-gpam-0100-wtr-38-gpa) (Agua/Residuos)
│   │   ├── ATA-39-PANEL/                       # [COAFI-GPAM-0100-PNL-39-GPA](#coafi-gpam-0100-pnl-39-gpa) (Paneles eléctricos/electrónicos)
│   │   ├── ATA-41-BALL/                        # [COAFI-GPAM-0100-BAL-41-GPA](#coafi-gpam-0100-bal-41-gpa) (Lastre de agua)
│   │   ├── ATA-42-IMA/                         # [COAFI-GPAM-0100-IMA-42-GPA](#coafi-gpam-0100-ima-42-gpa) (Arquitectura modular integrada)
│   │   ├── ATA-44-CABIN/                       # [COAFI-GPAM-0100-CAB-44-GPA](#coafi-gpam-0100-cab-44-gpa) (Sistemas de cabina)
│   │   ├── ATA-45-CMS/                         # [COAFI-GPAM-0100-CMS-45-GPA](#coafi-gpam-0100-cms-45-gpa) (Sistema de monitoreo central)
│   │   ├── ATA-46-INFO/                        # [COAFI-GPAM-0100-INF-46-GPA](#coafi-gpam-0100-inf-46-gpa) (Sistemas de información)
│   │   ├── ATA-47-NGS/                         # [COAFI-GPAM-0100-NGS-47-GPA](#coafi-gpam-0100-ngs-47-gpa) (Sistema de generación de nitrógeno)
│   │   ├── ATA-49-APU/                         # [COAFI-GPAM-0100-APU-49-GPA](#coafi-gpam-0100-apu-49-gpa) (Unidad de potencia auxiliar)
│   │   ├── ATA-50-CARGO/                       # [COAFI-GPAM-0100-CGO-50-GPA](#coafi-gpam-0100-cgo-50-gpa) (Compartimentos de carga)
│   │   ├── ATA-51-STRUCT/                      # [COAFI-GPAM-0100-STR-51-GPA](#coafi-gpam-0100-str-51-gpa) (Estructuras estándar)
│   │   ├── ATA-52-DOORS/                       # [COAFI-GPAM-0100-DOR-52-GPA](#coafi-gpam-0100-dor-52-gpa) (Puertas)
│   │   ├── ATA-53-FUSEL/                       # [COAFI-GPAM-0100-FSL-53-GPA](#coafi-gpam-0100-fsl-53-gpa) (Fuselaje)
│   │   ├── ATA-54-NACELLE/                     # [COAFI-GPAM-0100-NAC-54-GPA](#coafi-gpam-0100-nac-54-gpa) (Góndolas/Pilones)
│   │   ├── ATA-55-STAB/                        # [COAFI-GPAM-0100-STB-55-GPA](#coafi-gpam-0100-stb-55-gpa) (Estabilizadores)
│   │   ├── ATA-56-WINDOW/                      # [COAFI-GPAM-0100-WIN-56-GPA](#coafi-gpam-0100-win-56-gpa) (Ventanas)
│   │   ├── ATA-57-WING/                        # [COAFI-GPAM-0100-WNG-57-GPA](#coafi-gpam-0100-wng-57-gpa) (Alas)
│   │   ├── ATA-60-STD-ENG/                     # [COAFI-GPAM-0100-STE-60-GPA](#coafi-gpam-0100-ste-60-gpa) (Prácticas estándar - Motor)
│   │   ├── ATA-61-PROP/                        # [COAFI-GPAM-0100-PRP-61-GPA](#coafi-gpam-0100-prp-61-gpa) (Hélices/Propulsores)
│   │   ├── ATA-62-ROTOR/                       # [COAFI-GPAM-0100-RTR-62-GPA](#coafi-gpam-0100-rtr-62-gpa) (Rotores principales)
│   │   ├── ATA-63-ROTORDR/                     # [COAFI-GPAM-0100-RTD-63-GPA](#coafi-gpam-0100-rtd-63-gpa) (Transmisión del rotor principal)
│   │   ├── ATA-64-TAIL/                        # [COAFI-GPAM-0100-TLR-64-GPA](#coafi-gpam-0100-tlr-64-gpa) (Rotor de cola)
│   │   ├── ATA-65-TAILDR/                      # [COAFI-GPAM-0100-TLD-65-GPA](#coafi-gpam-0100-tld-65-gpa) (Transmisión del rotor de cola)
│   │   ├── ATA-66-FOLD/                        # [COAFI-GPAM-0100-FLD-66-GPA](#coafi-gpam-0100-fld-66-gpa) (Palas/Pilones plegables)
│   │   ├── ATA-67-ROTFC/                       # [COAFI-GPAM-0100-RFC-67-GPA](#coafi-gpam-0100-rfc-67-gpa) (Controles de vuelo del rotor)
│   │   ├── ATA-70-STD-ENG/                     # [COAFI-GPAM-0100-STE-70-GPA](#coafi-gpam-0100-ste-70-gpa) (Prácticas estándar - Motor)
│   │   ├── ATA-71-POWER/                       # [COAFI-GPAM-0100-PWR-71-GPA](#coafi-gpam-0100-pwr-71-gpa) (Planta de potencia)
│   │   ├── ATA-72-ENGINE/                      # [COAFI-GPAM-0100-ENG-72-GPA](#coafi-gpam-0100-eng-72-gpa) (Motor)
│   │   │   └── Q01/                            # [COAFI-GPAM-0100-QPE-72-GPA](#coafi-gpam-0100-qpe-72-gpa) (Cuestionario de motor)
│   │   ├── ATA-73-EFUEL/                       # [COAFI-GPAM-0100-EFL-73-GPA](#coafi-gpam-0100-efl-73-gpa) (Combustible del motor)
│   │   ├── ATA-74-IGN/                         # [COAFI-GPAM-0100-IGN-74-GPA](#coafi-gpam-0100-ign-74-gpa) (Ignición)
│   │   ├── ATA-75-AIR/                         # [COAFI-GPAM-0100-AIR-75-GPA](#coafi-gpam-0100-air-75-gpa) (Aire)
│   │   ├── ATA-76-CTRL/                        # [COAFI-GPAM-0100-CTL-76-GPA](#coafi-gpam-0100-ctl-76-gpa) (Controles del motor)
│   │   ├── ATA-77-IND/                         # [COAFI-GPAM-0100-IND-77-GPA](#coafi-gpam-0100-ind-77-gpa) (Indicación del motor)
│   │   ├── ATA-78-EXH/                         # [COAFI-GPAM-0100-EXH-78-GPA](#coafi-gpam-0100-exh-78-gpa) (Escape)
│   │   ├── ATA-79-OIL/                         # [COAFI-GPAM-0100-OIL-79-GPA](#coafi-gpam-0100-oil-79-gpa) (Aceite)
│   │   ├── ATA-80-START/                       # [COAFI-GPAM-0100-SRT-80-GPA](#coafi-gpam-0100-srt-80-gpa) (Arranque)
│   │   ├── ATA-83-GEAR/                        # [COAFI-GPAM-0100-AGB-83-GPA](#coafi-gpam-0100-agb-83-gpa) (Cajas de accesorios)
│   │   ├── ATA-85-FUEL-CELL/                   # [COAFI-GPAM-0100-FCL-85-GPA](#coafi-gpam-0100-fcl-85-gpa) (Celdas de combustible)
│   │   ├── ATA-91-CHART/                       # [COAFI-GPAM-0100-CHT-91-GPA](#coafi-gpam-0100-cht-91-gpa) (Diagramas)
│   │   ├── ATA-92-ELEC-INST/                   # [COAFI-GPAM-0100-ELI-92-GPA](#coafi-gpam-0100-eli-92-gpa) (Instalación eléctrica)
│   │   ├── ATA-95-GSE/                         # [COAFI-GPAM-0100-GSE-95-GPA](#coafi-gpam-0100-gse-95-gpa) (Equipo de apoyo en tierra)
│   │   ├── ATA-97-WIRE/                        # [COAFI-GPAM-0100-WIR-97-GPA](#coafi-gpam-0100-wir-97-gpa) (Registro de cableado)
│   │   └── ATA-99-SPECIAL/                     # [COAFI-GPAM-0100-SPC-99-GPA](#coafi-gpam-0100-spc-99-gpa) (Equipos especiales)
│   └── docs/                                   # [COAFI-GPAM-0000-DOC-00-GPA](#coafi-gpam-0000-doc-00-gpa) (Documentación)
│
├── GP-ATM/                                     # [COAFI-GPATM-0000-ATM-00-GPA](#coafi-gpatm-0000-atm-00-gpa) (Gestión del tráfico aéreo)
│   ├── README.md
│   ├── conventional/                           # [COAFI-GPATM-0200-CNV-00-GPA](#coafi-gpatm-0200-cnv-00-gpa) (Sistemas ATM convencionales)
│   ├── next-gen/                               # [COAFI-GPATM-0200-NXT-00-GPA](#coafi-gpatm-0200-nxt-00-gpa) (Sistemas ATM de próxima generación)
│   ├── integration/                            # [COAFI-GPATM-0200-INT-00-GPA](#coafi-gpatm-0200-int-00-gpa) (Integración de sistemas ATM)
│   └── docs/                                   # [COAFI-GPATM-0000-DOC-00-GPA](#coafi-gpatm-0000-doc-00-gpa) (Documentación)
│
├── GP-AERO/                                    # [COAFI-GPAERO-0000-AER-00-GPA](#coafi-gpaero-0000-aer-00-gpa) (Aerodinámica)
│   ├── README.md
│   ├── aerodynamics/                           # [COAFI-GPAERO-0300-ADY-00-GPA](#coafi-gpaero-0300-ady-00-gpa) (Principios aerodinámicos)
│   ├── propulsion/                             # [COAFI-GPAERO-0300-PRP-00-GPA](#coafi-gpaero-0300-prp-00-gpa) (Sistemas de propulsión)
│   ├── simulation/                             # [COAFI-GPAERO-0300-SIM-00-GPA](#coafi-gpaero-0300-sim-00-gpa) (Simulación aerodinámica)
│   └── docs/                                   # [COAFI-GPAERO-0000-DOC-00-GPA](#coafi-gpaero-0000-doc-00-gpa) (Documentación)
│
├── GP-AVIONICS/                                # [COAFI-GPAVI-0000-AVI-00-GPA](#coafi-gpavi-0000-avi-00-gpa) (Aviónica)
│   ├── README.md
│   ├── cockpit/                                # [COAFI-GPAVI-0400-CKP-00-GPA](#coafi-gpavi-0400-ckp-00-gpa) (Sistemas de cabina)
│   ├── flight-control/                         # [COAFI-GPAVI-0400-FCS-00-GPA](#coafi-gpavi-0400-fcs-00-gpa) (Sistemas de control de vuelo)
│   ├── navigation/                             # [COAFI-GPAVI-0400-NAV-00-GPA](#coafi-gpavi-0400-nav-00-gpa) (Sistemas de navegación)
│   ├── communication/                          # [COAFI-GPAVI-0400-COM-00-GPA](#coafi-gpavi-0400-com-00-gpa) (Sistemas de comunicación)
│   └── docs/                                   # [COAFI-GPAVI-0000-DOC-00-GPA](#coafi-gpavi-0000-doc-00-gpa) (Documentación)
│
├── GP-AERIAL-ROBOTICS/                         # [COAFI-GPARB-0000-ARB-00-GPA](#coafi-gparb-0000-arb-00-gpa) (Robótica aérea)
│   ├── README.md
│   ├── platforms/                              # [COAFI-GPARB-0500-PLT-00-GPA](#coafi-gparb-0500-plt-00-gpa) (Plataformas robóticas aéreas)
│   ├── swarm/                                  # [COAFI-GPARB-0500-SWM-00-GPA](#coafi-gparb-0500-swm-00-gpa) (Sistemas de enjambre aéreo)
��   ├── manipulation/                           # [COAFI-GPARB-0500-MNP-00-GPA](#coafi-gparb-0500-mnp-00-gpa) (Manipulación robótica aérea)
│   └── docs/                                   # [COAFI-GPARB-0000-DOC-00-GPA](#coafi-gparb-0000-doc-00-gpa) (Documentación)
│
└── GP-SENSATM/                                 # [COAFI-GPSAT-0000-SAT-00-GPA](#coafi-gpsat-0000-sat-00-gpa) (Sensores atmosféricos)
    ├── README.md
    ├── weather/                                # [COAFI-GPSAT-0600-WTH-00-GPA](#coafi-gpsat-0600-wth-00-gpa) (Sensores meteorológicos)
    ├── climate/                                # [COAFI-GPSAT-0600-CLM-00-GPA](#coafi-gpsat-0600-clm-00-gpa) (Monitoreo climático)
    ├── sensing/                                # [COAFI-GPSAT-0600-SNS-00-GPA](#coafi-gpsat-0600-sns-00-gpa) (Tecnologías de sensores)
    └── docs/                                   # [COAFI-GPSAT-0000-DOC-00-GPA](#coafi-gpsat-0000-doc-00-gpa) (Documentación)
```

## 5. GAIA-SPACEs Structure

```plaintext
GAIA-SPACEs/                                    # [COAFI-GSPC-0000-SPC-00-GPF](#coafi-gspc-0000-spc-00-gpf) (Plataformas espaciales y astronáuticas)
├── README.md
├── AToC.md                                     # [COAFI-GSPC-0000-TOC-00-GPF](#coafi-gspc-0000-toc-00-gpf) (Tabla de contenidos arquitectónica)
│
├── GP-AS/                                      # [COAFI-  (Tabla de contenidos arquitectónica)
│
├── GP-AS/                                      # [COAFI-GPAS-0000-AST-00-GPS](#coafi-gpas-0000-ast-00-gps) (Sistemas astronáuticos)
│   ├── README.md
│   ├── AMPELPLUS/                              # [COAFI-GPAS-0200-AMP-00-GPS](#coafi-gpas-0200-amp-00-gps) (Plataforma de modelado espacial)
│   │   ├── AS-00-GEN/                          # [COAFI-GPAS-0200-GEN-00-GPS](#coafi-gpas-0200-gen-00-gps) (Información general)
│   │   ├── AS-01-SC/                           # [COAFI-GPAS-0200-SCG-01-GPS](#coafi-gpas-0200-scg-01-gps) (Configuración de nave espacial)
│   │   ├── AS-02-OPS/                          # [COAFI-GPAS-0200-OPS-02-GPS](#coafi-gpas-0200-ops-02-gps) (Operaciones)
│   │   ├── AS-03-PERF/                         # [COAFI-GPAS-0200-PER-03-GPS](#coafi-gpas-0200-per-03-gps) (Rendimiento)
│   │   ├── AS-04-SAFETY/                       # [COAFI-GPAS-0200-SAF-04-GPS](#coafi-gpas-0200-saf-04-gps) (Seguridad)
│   │   ├── AS-05-MAINT/                        # [COAFI-GPAS-0200-MNT-05-GPS](#coafi-gpas-0200-mnt-05-gps) (Mantenimiento)
│   │   ├── AS-06-DIM/                          # [COAFI-GPAS-0200-DIM-06-GPS](#coafi-gpas-0200-dim-06-gps) (Dimensiones)
│   │   ├── AS-07-HAND/                         # [COAFI-GPAS-0200-HND-07-GPS](#coafi-gpas-0200-hnd-07-gps) (Manipulación)
│   │   ├── AS-08-MASS/                         # [COAFI-GPAS-0200-MAS-08-GPS](#coafi-gpas-0200-mas-08-gps) (Propiedades de masa)
│   │   ├── AS-09-LV/                           # [COAFI-GPAS-0200-LVI-09-GPS](#coafi-gpas-0200-lvi-09-gps) (Integración con vehículo lanzador)
│   │   ├── AS-10-STOW/                         # [COAFI-GPAS-0200-STW-10-GPS](#coafi-gpas-0200-stw-10-gps) (Almacenamiento)
│   │   ├── AS-11-MARK/                         # [COAFI-GPAS-0200-MRK-11-GPS](#coafi-gpas-0200-mrk-11-gps) (Marcas y etiquetas)
│   │   ├── AS-12-SERV/                         # [COAFI-GPAS-0200-SRV-12-GPS](#coafi-gpas-0200-srv-12-gps) (Servicio)
│   │   ├── AS-13-PROP/                         # [COAFI-GPAS-0200-PRP-13-GPS](#coafi-gpas-0200-prp-13-gps) (Propulsión)
│   │   ├── AS-14-PNEU/                         # [COAFI-GPAS-0200-PNU-14-GPS](#coafi-gpas-0200-pnu-14-gps) (Neumática)
│   │   ├── AS-15-THERM/                        # [COAFI-GPAS-0200-THM-15-GPS](#coafi-gpas-0200-thm-15-gps) (Control térmico)
│   │   ├── AS-16-RAD/                          # [COAFI-GPAS-0200-RAD-16-GPS](#coafi-gpas-0200-rad-16-gps) (Radiación)
│   │   ├── AS-17-CRYO/                         # [COAFI-GPAS-0200-CRY-17-GPS](#coafi-gpas-0200-cry-17-gps) (Criogenia)
│   │   ├── AS-18-ENV/                          # [COAFI-GPAS-0200-ENV-18-GPS](#coafi-gpas-0200-env-18-gps) (Entorno espacial)
│   │   ├── AS-19-STRUCT/                       # [COAFI-GPAS-0200-STR-19-GPS](#coafi-gpas-0200-str-19-gps) (Estructura)
│   │   ├── AS-20-STD/                          # [COAFI-GPAS-0200-STD-20-GPS](#coafi-gpas-0200-std-20-gps) (Estándares)
│   │   ├── AS-21-ECLSS/                        # [COAFI-GPAS-0200-ECL-21-GPS](#coafi-gpas-0200-ecl-21-gps) (Sistemas de soporte vital)
│   │   ├── AS-22-GNC/                          # [COAFI-GPAS-0200-GNC-22-GPS](#coafi-gpas-0200-gnc-22-gps) (Guiado, navegación y control)
│   │   ├── AS-23-COMM/                         # [COAFI-GPAS-0200-COM-23-GPS](#coafi-gpas-0200-com-23-gps) (Comunicaciones)
│   │   ├── AS-24-POWER/                        # [COAFI-GPAS-0200-PWR-24-GPS](#coafi-gpas-0200-pwr-24-gps) (Energía)
│   │   ├── AS-25-PAYLOAD/                      # [COAFI-GPAS-0200-PLD-25-GPS](#coafi-gpas-0200-pld-25-gps) (Carga útil)
│   │   ├── AS-26-FIRE/                         # [COAFI-GPAS-0200-FIR-26-GPS](#coafi-gpas-0200-fir-26-gps) (Protección contra incendios)
│   │   ├── AS-27-CTRL/                         # [COAFI-GPAS-0200-CTL-27-GPS](#coafi-gpas-0200-ctl-27-gps) (Control)
│   │   ├── AS-28-FUEL/                         # [COAFI-GPAS-0200-FUL-28-GPS](#coafi-gpas-0200-ful-28-gps) (Combustible)
│   │   ├── AS-29-HYDRA/                        # [COAFI-GPAS-0200-HYD-29-GPS](#coafi-gpas-0200-hyd-29-gps) (Hidráulica)
│   │   ├── AS-30-SHIELD/                       # [COAFI-GPAS-0200-SHD-30-GPS](#coafi-gpas-0200-shd-30-gps) (Blindaje)
│   │   ├── AS-31-INSTR/                        # [COAFI-GPAS-0200-INS-31-GPS](#coafi-gpas-0200-ins-31-gps) (Instrumentación)
│   │   ├── AS-32-LAND/                         # [COAFI-GPAS-0200-LND-32-GPS](#coafi-gpas-0200-lnd-32-gps) (Aterrizaje)
│   │   ├── AS-33-LIGHT/                        # [COAFI-GPAS-0200-LGT-33-GPS](#coafi-gpas-0200-lgt-33-gps) (Iluminación)
│   │   ├── AS-34-NAV/                          # [COAFI-GPAS-0200-NAV-34-GPS](#coafi-gpas-0200-nav-34-gps) (Navegación)
│   │   ├── AS-35-LIFE/                         # [COAFI-GPAS-0200-LIF-35-GPS](#coafi-gpas-0200-lif-35-gps) (Soporte vital)
│   │   ├── AS-36-DOCK/                         # [COAFI-GPAS-0200-DCK-36-GPS](#coafi-gpas-0200-dck-36-gps) (Acoplamiento)
│   │   ├── AS-37-ROBOT/                        # [COAFI-GPAS-0200-ROB-37-GPS](#coafi-gpas-0200-rob-37-gps) (Robótica)
│   │   ├── AS-38-WASTE/                        # [COAFI-GPAS-0200-WST-38-GPS](#coafi-gpas-0200-wst-38-gps) (Gestión de residuos)
│   │   ├── AS-39-COMP/                         # [COAFI-GPAS-0200-CMP-39-GPS](#coafi-gpas-0200-cmp-39-gps) (Computación)
│   │   ├── AS-40-DEPLOY/                       # [COAFI-GPAS-0200-DPL-40-GPS](#coafi-gpas-0200-dpl-40-gps) (Despliegue)
│   │   ├── AS-41-SCIENCE/                      # [COAFI-GPAS-0200-SCI-41-GPS](#coafi-gpas-0200-sci-41-gps) (Instrumentos científicos)
│   │   ├── AS-42-AVIONICS/                     # [COAFI-GPAS-0200-AVI-42-GPS](#coafi-gpas-0200-avi-42-gps) (Aviónica)
│   │   ├── AS-43-TELECOM/                      # [COAFI-GPAS-0200-TLC-43-GPS](#coafi-gpas-0200-tlc-43-gps) (Telecomunicaciones)
│   │   ├── AS-44-HABITAT/                      # [COAFI-GPAS-0200-HAB-44-GPS](#coafi-gpas-0200-hab-44-gps) (Hábitat)
│   │   ├── AS-45-DIAG/                         # [COAFI-GPAS-0200-DIA-45-GPS](#coafi-gpas-0200-dia-45-gps) (Diagnóstico)
│   │   ├── AS-46-INFO/                         # [COAFI-GPAS-0200-INF-46-GPS](#coafi-gpas-0200-inf-46-gps) (Sistemas de información)
│   │   ├── AS-47-REGEN/                        # [COAFI-GPAS-0200-REG-47-GPS](#coafi-gpas-0200-reg-47-gps) (Sistemas regenerativos)
│   │   ├── AS-48-ISRU/                         # [COAFI-GPAS-0200-ISR-48-GPS](#coafi-gpas-0200-isr-48-gps) (Utilización de recursos in-situ)
│   │   ├── AS-49-AUX/                          # [COAFI-GPAS-0200-AUX-49-GPS](#coafi-gpas-0200-aux-49-gps) (Sistemas auxiliares)
│   │   ├── AS-50-CARGO/                        # [COAFI-GPAS-0200-CGO-50-GPS](#coafi-gpas-0200-cgo-50-gps) (Carga)
│   │   ├── AS-51-STRUCT/                       # [COAFI-GPAS-0200-STR-51-GPS](#coafi-gpas-0200-str-51-gps) (Estructura)
│   │   ├── AS-52-HATCH/                        # [COAFI-GPAS-0200-HTC-52-GPS](#coafi-gpas-0200-htc-52-gps) (Escotillas)
│   │   ├── AS-53-SHELL/                        # [COAFI-GPAS-0200-SHL-53-GPS](#coafi-gpas-0200-shl-53-gps) (Casco/Estructura externa)
│   │   ├── AS-54-MOUNT/                        # [COAFI-GPAS-0200-MNT-54-GPS](#coafi-gpas-0200-mnt-54-gps) (Montajes)
│   │   ├── AS-55-SOLAR/                        # [COAFI-GPAS-0200-SOL-55-GPS](#coafi-gpas-0200-sol-55-gps) (Paneles solares)
│   │   ├── AS-56-WINDOW/                       # [COAFI-GPAS-0200-WIN-56-GPS](#coafi-gpas-0200-win-56-gps) (Ventanas)
│   │   ├── AS-57-RADIATOR/                     # [COAFI-GPAS-0200-RAD-57-GPS](#coafi-gpas-0200-rad-57-gps) (Radiadores)
│   │   ├── AS-58-THERMAL/                      # [COAFI-GPAS-0200-THR-58-GPS](#coafi-gpas-0200-thr-58-gps) (Control térmico)
│   │   ├── AS-59-INSUL/                        # [COAFI-GPAS-0200-INS-59-GPS](#coafi-gpas-0200-ins-59-gps) (Aislamiento)
│   │   ├── AS-60-STD-PROP/                     # [COAFI-GPAS-0200-STP-60-GPS](#coafi-gpas-0200-stp-60-gps) (Estándares de propulsión)
│   │   ├── AS-61-MAIN-ENG/                     # [COAFI-GPAS-0200-MEN-61-GPS](#coafi-gpas-0200-men-61-gps) (Motor principal)
│   │   ├── AS-62-RCS/                          # [COAFI-GPAS-0200-RCS-62-GPS](#coafi-gpas-0200-rcs-62-gps) (Sistema de control de reacción)
│   │   ├── AS-63-ELEC-PROP/                    # [COAFI-GPAS-0200-EPR-63-GPS](#coafi-gpas-0200-epr-63-gps) (Propulsión eléctrica)
│   │   ├── AS-64-NUC-PROP/                     # [COAFI-GPAS-0200-NPR-64-GPS](#coafi-gpas-0200-npr-64-gps) (Propulsión nuclear)
│   │   ├── AS-65-SOLAR-SAIL/                   # [COAFI-GPAS-0200-SSL-65-GPS](#coafi-gpas-0200-ssl-65-gps) (Vela solar)
│   │   ├── AS-66-TETHER/                       # [COAFI-GPAS-0200-TTH-66-GPS](#coafi-gpas-0200-tth-66-gps) (Sistemas de amarre)
│   │   ├── AS-67-PROP-CTRL/                    # [COAFI-GPAS-0200-PCT-67-GPS](#coafi-gpas-0200-pct-67-gps) (Control de propulsión)
│   │   ├── AS-68-PROP-TANK/                    # [COAFI-GPAS-0200-PTK-68-GPS](#coafi-gpas-0200-ptk-68-gps) (Tanques de propulsión)
│   │   ├── AS-69-PROP-FEED/                    # [COAFI-GPAS-0200-PFD-69-GPS](#coafi-gpas-0200-pfd-69-gps) (Alimentación de propulsión)
│   │   ├── AS-70-STD-POWER/                    # [COAFI-GPAS-0200-SPW-70-GPS](#coafi-gpas-0200-spw-70-gps) (Estándares de energía)
│   │   ├── AS-71-POWER-GEN/                    # [COAFI-GPAS-0200-PWG-71-GPS](#coafi-gpas-0200-pwg-71-gps) (Generación de energía)
│   │   ├── AS-72-POWER-STOR/                   # [COAFI-GPAS-0200-PWS-72-GPS](#coafi-gpas-0200-pws-72-gps) (Almacenamiento de energía)
│   │   ├── AS-73-POWER-DIST/                   # [COAFI-GPAS-0200-PWD-73-GPS](#coafi-gpas-0200-pwd-73-gps) (Distribución de energía)
│   │   ├── AS-74-POWER-CTRL/                   # [COAFI-GPAS-0200-PWC-74-GPS](#coafi-gpas-0200-pwc-74-gps) (Control de energía)
│   │   ├── AS-75-POWER-COND/                   # [COAFI-GPAS-0200-PWN-75-GPS](#coafi-gpas-0200-pwn-75-gps) (Acondicionamiento de energía)
│   │   ├── AS-76-FUEL-CELL/                    # [COAFI-GPAS-0200-FCL-76-GPS](#coafi-gpas-0200-fcl-76-gps) (Celdas de combustible)
│   │   ├── AS-77-NUCLEAR/                      # [COAFI-GPAS-0200-NUC-77-GPS](#coafi-gpas-0200-nuc-77-gps) (Energía nuclear)
│   │   ├── AS-78-RTG/                          # [COAFI-GPAS-0200-RTG-78-GPS](#coafi-gpas-0200-rtg-78-gps) (Generador termoeléctrico de radioisótopos)
│   │   ├── AS-79-SOLAR-ARR/                    # [COAFI-GPAS-0200-SAR-79-GPS](#coafi-gpas-0200-sar-79-gps) (Matrices solares)
│   │   ├── AS-80-BATT/                         # [COAFI-GPAS-0200-BAT-80-GPS](#coafi-gpas-0200-bat-80-gps) (Baterías)
│   │   ├── AS-81-FLYWHEEL/                     # [COAFI-GPAS-0200-FLW-81-GPS](#coafi-gpas-0200-flw-81-gps) (Volantes de inercia)
│   │   ├── AS-82-SUPER-CAP/                    # [COAFI-GPAS-0200-SCP-82-GPS](#coafi-gpas-0200-scp-82-gps) (Supercapacitores)
│   │   ├── AS-83-POWER-MGMT/                   # [COAFI-GPAS-0200-PWM-83-GPS](#coafi-gpas-0200-pwm-83-gps) (Gestión de energía)
│   │   ├── AS-84-POWER-SAFE/                   # [COAFI-GPAS-0200-PWF-84-GPS](#coafi-gpas-0200-pwf-84-gps) (Seguridad energética)
│   │   ├── AS-85-POWER-EMER/                   # [COAFI-GPAS-0200-PWE-85-GPS](#coafi-gpas-0200-pwe-85-gps) (Energía de emergencia)
│   │   ├── AS-86-POWER-GRND/                   # [COAFI-GPAS-0200-PWG-86-GPS](#coafi-gpas-0200-pwg-86-gps) (Energía en tierra)
│   │   ├── AS-87-POWER-TEST/                   # [COAFI-GPAS-0200-PWT-87-GPS](#coafi-gpas-0200-pwt-87-gps) (Pruebas de energía)
│   │   ├── AS-88-POWER-INTFC/                  # [COAFI-GPAS-0200-PWI-88-GPS](#coafi-gpas-0200-pwi-88-gps) (Interfaces de energía)
│   │   ├── AS-89-POWER-REDUN/                  # [COAFI-GPAS-0200-PWR-89-GPS](#coafi-gpas-0200-pwr-89-gps) (Redundancia energética)
│   │   ├── AS-90-COMM-STD/                     # [COAFI-GPAS-0200-CMS-90-GPS](#coafi-gpas-0200-cms-90-gps) (Estándares de comunicación)
│   │   ├── AS-91-COMM-RF/                      # [COAFI-GPAS-0200-CRF-91-GPS](#coafi-gpas-0200-crf-91-gps) (Comunicación por radiofrecuencia)
│   │   ├── AS-92-COMM-OPT/                     # [COAFI-GPAS-0200-COP-92-GPS](#coafi-gpas-0200-cop-92-gps) (Comunicación óptica)
│   │   ├── AS-93-COMM-LASER/                   # [COAFI-GPAS-0200-CLS-93-GPS](#coafi-gpas-0200-cls-93-gps) (Comunicación láser)
│   │   ├── AS-94-COMM-CRYPTO/                  # [COAFI-GPAS-0200-CCR-94-GPS](#coafi-gpas-0200-ccr-94-gps) (Criptografía de comunicaciones)
│   │   ├── AS-95-COMM-PROTO/                   # [COAFI-GPAS-0200-CPR-95-GPS](#coafi-gpas-0200-cpr-95-gps) (Protocolos de comunicación)
│   │   ├── AS-96-COMM-ANTEN/                   # [COAFI-GPAS-0200-CAN-96-GPS](#coafi-gpas-0200-can-96-gps) (Antenas de comunicación)
│   │   ├── AS-97-COMM-NETW/                    # [COAFI-GPAS-0200-CNT-97-GPS](#coafi-gpas-0200-cnt-97-gps) (Redes de comunicación)
│   │   ├── AS-98-COMM-SECU/                    # [COAFI-GPAS-0200-CSC-98-GPS](#coafi-gpas-0200-csc-98-gps) (Seguridad de comunicaciones)
│   │   └── AS-99-SPECIAL/                      # [COAFI-GPAS-0200-SPC-99-GPS](#coafi-gpas-0200-spc-99-gps) (Equipos especiales)
│   └── docs/                                   # [COAFI-GPAS-0000-DOC-00-GPS](#coafi-gpas-0000-doc-00-gps) (Documentación)
│
├── GP-EXPLORATION/                             # [COAFI-GPEXP-0000-EXP-00-GPS](#coafi-gpexp-0000-exp-00-gps) (Exploración espacial)
│   ├── README.md
│   ├── lunar/                                  # [COAFI-GPEXP-0300-LUN-00-GPS](#coafi-gpexp-0300-lun-00-gps) (Exploración lunar)
│   ├── mars/                                   # [COAFI-GPEXP-0300-MRS-00-GPS](#coafi-gpexp-0300-mrs-00-gps) (Exploración marciana)
│   ├── asteroid/                               # [COAFI-GPEXP-0300-AST-00-GPS](#coafi-gpexp-0300-ast-00-gps) (Exploración de asteroides)
│   ├── deep-space/                             # [COAFI-GPEXP-0300-DSP-00-GPS](#coafi-gpexp-0300-dsp-00-gps) (Exploración del espacio profundo)
│   └── docs/                                   # [COAFI-GPEXP-0000-DOC-00-GPS](#coafi-gpexp-0000-doc-00-gps) (Documentación)
│
├── GP-HABITATS/                                # [COAFI-GPHAB-0000-HAB-00-GPS](#coafi-gphab-0000-hab-00-gps) (Hábitats espaciales)
│   ├── README.md
│   ├── life-support/                           # [COAFI-GPHAB-0400-LFS-00-GPS](#coafi-gphab-0400-lfs-00-gps) (Sistemas de soporte vital)
│   ├── habitation/                             # [COAFI-GPHAB-0400-HBT-00-GPS](#coafi-gphab-0400-hbt-00-gps) (Módulos de habitación)
│   ├── space-stations/                         # [COAFI-GPHAB-0400-STA-00-GPS](#coafi-gphab-0400-sta-00-gps) (Estaciones espaciales)
│   ├── lunar-bases/                            # [COAFI-GPHAB-0400-LBS-00-GPS](#coafi-gphab-0400-lbs-00-gps) (Bases lunares)
│   └── docs/                                   # [COAFI-GPHAB-0000-DOC-00-GPS](#coafi-gphab-0000-doc-00-gps) (Documentación)
│
├── GP-ORBITAL/                                 # [COAFI-GPORB-0000-ORB-00-GPS](#coafi-gporb-0000-orb-00-gps) (Operaciones orbitales)
│   ├── README.md
│   ├── debris/                                 # [COAFI-GPORB-0500-DEB-00-GPS](#coafi-gporb-0500-deb-00-gps) (Gestión de desechos espaciales)
│   ├── traffic/                                # [COAFI-GPORB-0500-TRF-00-GPS](#coafi-gporb-0500-trf-00-gps) (Gestión del tráfico orbital)
│   ├── servicing/                              # [COAFI-GPORB-0500-SRV-00-GPS](#coafi-gporb-0500-srv-00-gps) (Servicios en órbita)
│   └── docs/                                   # [COAFI-GPORB-0000-DOC-00-GPS](#coafi-gporb-0000-doc-00-gps) (Documentación)
│
├── GP-PROPULSION/                              # [COAFI-GPPRO-0000-PRO-00-GPS](#coafi-gppro-0000-pro-00-gps) (Propulsión espacial)
│   ├── README.md
│   ├── chemical/                               # [COAFI-GPPRO-0600-CHM-00-GPS](#coafi-gppro-0600-chm-00-gps) (Propulsión química)
│   ├── electric/                               # [COAFI-GPPRO-0600-ELC-00-GPS](#coafi-gppro-0600-elc-00-gps) (Propulsión eléctrica)
│   ├── nuclear/                                # [COAFI-GPPRO-0600-NUC-00-GPS](#coafi-gppro-0600-nuc-00-gps) (Propulsión nuclear)
│   ├── quantum/                                # [COAFI-GPPRO-0600-QNT-00-GPS](#coafi-gppro-0600-qnt-00-gps) (Propulsión cuántica)
│   └── docs/                                   # [COAFI-GPPRO-0000-DOC-00-GPS](#coafi-gppro-0000-doc-00-gps) (Documentación)
│
└── GP-ASTRO-ROBOTICS/                          # [COAFI-GPARB-0000-ARB-00-GPS](#coafi-gparb-0000-arb-00-gps) (Robótica astronáutica)
    ├── README.md
    ├── servicing/                              # [COAFI-GPARB-0700-SRV-00-GPS](#coafi-gparb-0700-srv-00-gps) (Servicios robóticos)
    ├── assembly/                               # [COAFI-GPARB-0700-ASM-00-GPS](#coafi-gparb-0700-asm-00-gps) (Ensamblaje robótico)
    ├── exploration/                            # [COAFI-GPARB-0700-EXP-00-GPS](#coafi-gparb-0700-exp-00-gps) (Exploración robótica)
    └── docs/                                   # [COAFI-GPARB-0000-DOC-00-GPS](#coafi-gparb-0000-doc-00-gps) (Documentación)
```

## 6. GAIA-GROUND Structure

```plaintext
GAIA-GROUND/                                    # [COAFI-GGND-0000-GND-00-GPF](#coafi-ggnd-0000-gnd-00-gpf) (Infraestructura terrestre)
├── README.md
├── AToC.md                                     # [COAFI-GGND-0000-TOC-00-GPF](#coafi-ggnd-0000-toc-00-gpf) (Tabla de contenidos arquitectónica)
│
├── GP-AIRPORT/                                 # [COAFI-GPAIR-0000-AIR-00-GPG](#coafi-gpair-0000-air-00-gpg) (Infraestructura aeroportuaria)
│   ├── README.md
│   ├── AMPELGROUND/                            # [COAFI-GPAIR-1400-AMP-00-GPG](#coafi-gpair-1400-amp-00-gpg) (Plataforma de modelado aeroportuario)
│   │   ├── GI-00-GEN/                          # [COAFI-GPAIR-1400-GEN-00-GPG](#coafi-gpair-1400-gen-00-gpg) (Información general)
│   │   ├── GI-01-TERM/                         # [COAFI-GPAIR-1400-TRM-01-GPG](#coafi-gpair-1400-trm-01-gpg) (Terminal)
│   │   ├── GI-02-RUNW/                         # [COAFI-GPAIR-1400-RNW-02-GPG](#coafi-gpair-1400-rnw-02-gpg) (Pistas)
│   │   ├── GI-03-APRON/                        # [COAFI-GPAIR-1400-APR-03-GPG](#coafi-gpair-1400-apr-03-gpg) (Plataforma)
│   │   ├── GI-04-FUEL/                         # [COAFI-GPAIR-1400-FUL-04-GPG](#coafi-gpair-1400-ful-04-gpg) (Combustible)
│   │   ├── GI-05-CARGO/                        # [COAFI-GPAIR-1400-CRG-05-GPG](#coafi-gpair-1400-crg-05-gpg) (Carga)
│   │   ├── GI-06-MAINT/                        # [COAFI-GPAIR-1400-MNT-06-GPG](#coafi-gpair-1400-mnt-06-gpg) (Mantenimiento)
│   │   ├── GI-07-EMER/                         # [COAFI-GPAIR-1400-EMR-07-GPG](#coafi-gpair-1400-emr-07-gpg) (Emergencia)
│   │   ├── GI-08-SEC/                          # [COAFI-GPAIR-1400-SEC-08-GPG](#coafi-gpair-1400-sec-08-gpg) (Seguridad)
│   │   ├── GI-09-ENV/                          # [COAFI-GPAIR-1400-ENV-09-GPG](#coafi-gpair-1400-env-09-gpg) (Medio ambiente)
│   │   ├── GI-10-UTIL/                         # [COAFI-GPAIR-1400-UTL-10-GPG](#coafi-gpair-1400-utl-10-gpg) (Utilidades)
│   │   ├── GI-11-ACCESS/                       # [COAFI-GPAIR-1400-ACS-11-GPG](#coafi-gpair-1400-acs-11-gpg) (Acceso)
│   │   ├── GI-12-LIGHT/                        # [COAFI-GPAIR-1400-LGT-12-GPG](#coafi-gpair-1400-lgt-12-gpg) (Iluminación)
│   │   ├── GI-13-DRAIN/                        # [COAFI-GPAIR-1400-DRN-13-GPG](#coafi-gpair-1400-drn-13-gpg) (Drenaje)
│   │   ├── GI-14-PAVE/                         # [COAFI-GPAIR-1400-PAV-14-GPG](#coafi-gpair-1400-pav-14-gpg) (Pavimentación)
│   │   ├── GI-15-MARK/                         # [COAFI-GPAIR-1400-MRK-15-GPG](#coafi-gpair-1400-mrk-15-gpg) (Marcas)
│   │   └── GI-16-PLAN/                         # [COAFI-GPAIR-1400-PLN-16-GPG](#coafi-gpair-1400-pln-16-gpg) (Planificación)
│   └── docs/                                   # [COAFI-GPAIR-0000-DOC-00-GPG](#coafi-gpair-0000-doc-00-gpg) (Documentación)
│
├── GP-ATC/                                     # [COAFI-GPATC-0000-ATC-00-GPG](#coafi-gpatc-0000-atc-00-gpg) (Control de tráfico aéreo)
│   ├── README.md
│   ├── ATCGROUND/                              # [COAFI-GPATC-1500-ATC-00-GPG](#coafi-gpatc-1500-atc-00-gpg) (Sistemas de control de tráfico aéreo)
│   │   ├── GI-20-TWR/                          # [COAFI-GPATC-1500-TWR-20-GPG](#coafi-gpatc-1500-twr-20-gpg) (Torre)
│   │   ├── GI-21-APP/                          # [COAFI-GPATC-1500-APP-21-GPG](#coafi-gpatc-1500-app-21-gpg) (Aproximación)
│   │   ├── GI-22-ACC/                          # [COAFI-GPATC-1500-ACC-22-GPG](#coafi-gpatc-1500-acc-22-gpg) (Centro de control de área)
│   │   ├── GI-23-RADAR/                        # [COAFI-GPATC-1500-RDR-23-GPG](#coafi-gpatc-1500-rdr-23-gpg) (Radar)
│   │   ├── GI-24-COMM/                         # [COAFI-GPATC-1500-COM-24-GPG](#coafi-gpatc-1500-com-24-gpg) (Comunicaciones)
│   │   ├── GI-25-NAV/                          # [COAFI-GPATC-1500-NAV-25-GPG](#coafi-gpatc-1500-nav-25-gpg) (Navegación)
│   │   ├── GI-26-MET/                          # [COAFI-GPATC-1500-MET-26-GPG](#coafi-gpatc-1500-met-26-gpg) (Meteorología)
│   │   ├── GI-27-AUTO/                         # [COAFI-GPATC-1500-AUT-27-GPG](#coafi-gpatc-1500-aut-27-gpg) (Automatización)
│   │   └── GI-28-TRAIN/                        # [COAFI-GPATC-1500-TRN-28-GPG](#coafi-gpatc-1500-trn-28-gpg) (Entrenamiento)
│   └── docs/                                   # [COAFI-GPATC-0000-DOC-00-GPG](#coafi-gpatc-0000-doc-00-gpg) (Documentación)
│
├── GP-GSE/                                     # [COAFI-GPGSE-0000-GSE-00-GPG](#coafi-gpgse-0000-gse-00-gpg) (Equipo de apoyo en tierra)
│   ├── README.md
│   ├── GSEGROUND/                              # [COAFI-GPGSE-1600-GSE-00-GPG](#coafi-gpgse-1600-gse-00-gpg) (Sistemas de equipo de apoyo en tierra)
│   │   ├── GI-30-POWER/                        # [COAFI-GPGSE-1600-PWR-30-GPG](#coafi-gpgse-1600-pwr-30-gpg) (Energía)
│   │   ├── GI-31-AIR/                          # [COAFI-GPGSE-1600-AIR-31-GPG](#coafi-gpgse-1600-air-31-gpg) (Aire)
│   │   ├── GI-32-FUEL/                         # [COAFI-GPGSE-1600-FUL-32-GPG](#coafi-gpgse-1600-ful-32-gpg) (Combustible)
│   │   ├── GI-33-TOW/                          # [COAFI-GPGSE-1600-TOW-33-GPG](#coafi-gpgse-1600-tow-33-gpg) (Remolque)
│   │   ├── GI-34-LOAD/                         # [COAFI-GPGSE-1600-LOD-34-GPG](#coafi-gpgse-1600-lod-34-gpg) (Carga)
│   │   ├── GI-35-DEICE/                        # [COAFI-GPGSE-1600-ICE-35-GPG](#coafi-gpgse-1600-ice-35-gpg) (Deshielo)
│   │   ├── GI-36-MAINT/                        # [COAFI-GPGSE-1600-MNT-36-GPG](#coafi-gpgse-1600-mnt-36-gpg) (Mantenimiento)
│   │   ├── GI-37-TEST/                         # [COAFI-GPGSE-1600-TST-37-GPG](#coafi-gpgse-1600-tst-37-gpg) (Pruebas)
│   │   └── GI-38-SPEC/                         # [COAFI-GPGSE-1600-SPC-38-GPG](#coafi-gpgse-1600-spc-38-gpg) (Especial)
│   └── docs/                                   # [COAFI-GPGSE-0000-DOC-00-GPG](#coafi-gpgse-0000-doc-00-gpg) (Documentación)
│
├── GP-SPACEPORT/                               # [COAFI-GPSPT-0000-SPT-00-GPG](#coafi-gpspt-0000-spt-00-gpg) (Puerto espacial)
│   ├── README.md
│   ├── SPACEGROUND/                            # [COAFI-GPSPT-1700-SPT-00-GPG](#coafi-gpspt-1700-spt-00-gpg) (Sistemas de puerto espacial)
│   │   ├── GI-40-GEN/                          # [COAFI-GPSPT-1700-GEN-40-GPG](#coafi-gpspt-1700-gen-40-gpg) (General)
│   │   ├── GI-41-LAUNCH/                       # [COAFI-GPSPT-1700-LCH-41-GPG](#coafi-gpspt-1700-lch-41-gpg) (Lanzamiento)
│   │   ├── GI-42-INTEG/                        # [COAFI-GPSPT-1700-INT-42-GPG](#coafi-gpspt-1700-int-42-gpg) (Integración)
│   │   ├── GI-43-FUEL/                         # [COAFI-GPSPT-1700-FUL-43-GPG](#coafi-gpspt-1700-ful-43-gpg) (Combustible)
│   │   ├── GI-44-TRACK/                        # [COAFI-GPSPT-1700-TRK-44-GPG](#coafi-gpspt-1700-trk-44-gpg) (Seguimiento)
│   │   ├── GI-45-RECOV/                        # [COAFI-GPSPT-1700-RCV-45-GPG](#coafi-gpspt-1700-rcv-45-gpg) (Recuperación)
│   │   ├── GI-46-SAFE/                         # [COAFI-GPSPT-1700-SAF-46-GPG](#coafi-gpspt-1700-saf-46-gpg) (Seguridad)
│   │   └── GI-47-PAYLOAD/                      # [COAFI-GPSPT-1700-PLD-47-GPG](#coafi-gpspt-1700-pld-47-gpg) (Carga útil)
│   └── docs/                                   # [COAFI-GPSPT-0000-DOC-00-GPG](#coafi-gpspt-0000-doc-00-gpg) (Documentación)
│
└── GP-SMART-INFRA/                             # [COAFI-GPSMI-0000-SMI-00-GPG](#coafi-gpsmi-0000-smi-00-gpg) (Infraestructura inteligente)
    ├── README.md
    ├── SMARTGROUND/                            # [COAFI-GPSMI-1800-SMI-00-GPG](#coafi-gpsmi-1800-smi-00-gpg) (Sistemas de infraestructura inteligente)
    │   ├── GI-50-GEN/                          # [COAFI-GPSMI-1800-GEN-50-GPG](#coafi-gpsmi-1800-gen-50-gpg) (General)
    │   ├── GI-51-IOT/                          # [COAFI-GPSMI-1800-IOT-51-GPG](#coafi-gpsmi-1800-iot-51-gpg) (Internet de las cosas)
    │   ├── GI-52-AUTO/                         # [COAFI-GPSMI-1800-AUT-52-GPG](#coafi-gpsmi-1800-aut-52-gpg) (Automatización)
    │   ├── GI-53-ENERGY/                       # [COAFI-GPSMI-1800-ENG-53-GPG](#coafi-gpsmi-1800-eng-53-gpg) (Energía)
    │   ├── GI-54-DATA/                         # [COAFI-GPSMI-1800-DAT-54-GPG](#coafi-gpsmi-1800-dat-54-gpg) (Datos)
    │   ├── GI-55-CYBER/                        # [COAFI-GPSMI-1800-CYB-55-GPG](#coafi-gpsmi-1800-cyb-55-gpg) (Ciberseguridad)
    │   ├── GI-56-DIGITAL/                      # [COAFI-GPSMI-1800-DIG-56-GPG](#coafi-gpsmi-1800-dig-56-gpg) (Digitalización)
    │   ├── GI-57-AI/                           # [COAFI-GPSMI-1800-AII-57-GPG](#coafi-gpsmi-1800-aii-57-gpg) (Inteligencia artificial)
    │   └── GI-58-SUSTAIN/                      # [COAFI-GPSMI-1800-SUS-58-GPG](#coafi-gpsmi-1800-sus-58-gpg) (Sostenibilidad)
    └── docs/                                   # [COAFI-GPSMI-0000-DOC-00-GPG](#coafi-gpsmi-0000-doc-00-gpg) (Documentación)
```

## 7. GAIA-GREEN-TECHNOLOGIES Structure

```plaintext
GAIA-GREEN-TECHNOLOGIES/                        # [COAFI-GGRN-0000-GRN-00-GPF](#coafi-ggrn-0000-grn-00-gpf) (Tecnologías sostenibles)
├── README.md
├── AToC.md                                     # [COAFI-GGRN-0000-TOC-00-GPF](#coafi-ggrn-0000-toc-00-gpf) (Tabla de contenidos arquitectónica)
│
├── GP-GREEN-PROPULSION/                        # [COAFI-GPGRP-0000-GRP-00-GPG](#coafi-gpgrp-0000-grp-00-gpg) (Propulsión ecológica)
│   ├── README.md
│   ├── hydrogen/                               # [COAFI-GPGRP-2000-HYD-00-GPG](#coafi-gpgrp-2000-hyd-00-gpg) (Propulsión de hidrógeno)
│   ├── electric/                               # [COAFI-GPGRP-2000-ELC-00-GPG](#coafi-gpgrp-2000-elc-00-gpg) (Propulsión eléctrica)
│   ├── biofuel/                                # [COAFI-GPGRP-2000-BIO-00-GPG](#coafi-gpgrp-2000-bio-00-gpg) (Biocombustibles)
│   ├── hybrid/                                 # [COAFI-GPGRP-2000-HYB-00-GPG](#coafi-gpgrp-2000-hyb-00-gpg) (Sistemas híbridos)
│   └── docs/                                   # [COAFI-GPGRP-0000-DOC-00-GPG](#coafi-gpgrp-0000-doc-00-gpg) (Documentación)
│
├── GP-SMART-MATERIALS/                         # [COAFI-GPSMT-0000-SMT-00-GPG](#coafi-gpsmt-0000-smt-00-gpg) (Materiales inteligentes)
│   ├── README.md
│   ├── composites/                             # [COAFI-GPSMT-2100-CMP-00-GPG](#coafi-gpsmt-2100-cmp-00-gpg) (Materiales compuestos)
│   ├── self-healing/                           # [COAFI-GPSMT-2100-SLF-00-GPG](#coafi-gpsmt-2100-slf-00-gpg) (Materiales autorreparables)
│   ├── biomimetic/                             # [COAFI-GPSMT-2100-BIO-00-GPG](#coafi-gpsmt-2100-bio-00-gpg) (Materiales biomiméticos)
│   ├── manufacturing/                          # [COAFI-GPSMT-2100-MFG-00-GPG](#coafi-gpsmt-2100-mfg-00-gpg) (Fabricación avanzada)
│   └── docs/                                   # [COAFI-GPSMT-0000-DOC-00-GPG](#coafi-gpsmt-0000-doc-00-gpg) (Documentación)
│
├── GP-ENERGY/                                  # [COAFI-GPENG-0000-ENG-00-GPG](#coafi-gpeng-0000-eng-00-gpg) (Energía sostenible)
│   ├── README.md
│   ├── generation/                             # [COAFI-GPENG-2200-GEN-00-GPG](#coafi-gpeng-2200-gen-00-gpg) (Generación de energía)
│   ├── storage/                                # [COAFI-GPENG-2200-STR-00-GPG](#coafi-gpeng-2200-str-00-gpg) (Almacenamiento de energía)
│   ├── distribution/                           # [COAFI-GPENG-2200-DST-00-GPG](#coafi-gpeng-2200-dst-00-gpg) (Distribución de energía)
│   ├── management/                             # [COAFI-GPENG-2200-MGT-00-GPG](#coafi-gpeng-2200-mgt-00-gpg) (Gestión de energía)
│   └── docs/                                   # [COAFI-GPENG-0000-DOC-00-GPG](#coafi-gpeng-0000-doc-00-gpg) (Documentación)
│
├── GP-CIRCULAR/                                # [COAFI-GPCIR-0000-CIR-00-GPG](#coafi-gpcir-0000-cir-00-gpg) (Economía circular)
│   ├── README.md
│   ├── closed-loop/                            # [COAFI-GPCIR-2300-CLS-00-GPG](#coafi-gpcir-2300-cls-00-gpg) (Sistemas de ciclo cerrado)
│   ├── waste/                                  # [COAFI-GPCIR-2300-WST-00-GPG](#coafi-gpcir-2300-wst-00-gpg) (Gestión de residuos)
│   ├── recovery/                               # [COAFI-GPCIR-2300-RCV-00-GPG](#coafi-gpcir-2300-rcv-00-gpg) (Recuperación de materiales)
│   └── docs/                                   # [COAFI-GPCIR-0000-DOC-00-GPG](#coafi-gpcir-0000-doc-00-gpg) (Documentación)
│
├── GP-ENVIRO/                                  # [COAFI-GPENV-0000-ENV-00-GPG](#coafi-gpenv-0000-env-00-gpg) (Medio ambiente)
│   ├── README.md
│   ├── ecosystem/                              # [COAFI-GPENV-2400-ECO-00-GPG](#coafi-gpenv-2400-eco-00-gpg) (Ecosistemas)
│   ├── climate/                                # [COAFI-GPENV-2400-CLM-00-GPG](#coafi-gpenv-2400-clm-00-gpg) (Clima)
│   ├── biodiversity/                           # [COAFI-GPENV-2400-BIO-00-GPG](#coafi-gpenv-2400-bio-00-gpg) (Biodiversidad)
│   └── docs/                                   # [COAFI-GPENV-0000-DOC-00-GPG](#coafi-gpenv-0000-doc-00-gpg) (Documentación)
│
└── GP-REGEN/                                   # [COAFI-GPREG-0000-REG-00-GPG](#coafi-gpreg-0000-reg-00-gpg) (Diseño regenerativo)
    ├── README.md
    ├── principles/                             # [COAFI-GPREG-2500-PRI-00-GPG](#coafi-gpreg-2500-pri-00-gpg) (Principios regenerativos)
    ├── implementations/                         # [COAFI-GPREG-2500-IMP-00-GPG](#coafi-gpreg-2500-imp-00-gpg) (Implementaciones)
    ├── metrics/                                # [COAFI-GPREG-2500-MET-00-GPG](#coafi-gpreg-2500-met-00-gpg) (Métricas)
    └── docs/                                   # [COAFI-GPREG-0000-DOC-00-GPG](#coafi-gpreg-0000-doc-00-gpg) (Documentación)
```

## 8. SharedServices Structure

```plaintext
SharedServices/                                 # [COAFI-SSRV-0000-SRV-00-GPF](#coafi-ssrv-0000-srv-00-gpf) (Servicios compartidos)
├── README.md
│
├── GP-COM/                                     # [COAFI-GPCOM-0000-COM-00-GPC](#coafi-gpcom-0000-com-00-gpc) (Comunicaciones)
│   ├── README.md
│   ├── GEN/                                    # [COAFI-GPCOM-0300-GEN-00-GPC](#coafi-gpcom-0300-gen-00-gpc) (General)
│   │   └── CH-00/                              # [COAFI-GPCOM-0300-GEN-00-GPC](#coafi-gpcom-0300-gen-00-gpc) (Capítulo general)
│   ├── AI/                                     # [COAFI-GPCOM-0300-AIC-01-GPC](#coafi-gpcom-0300-aic-01-gpc) (Inteligencia artificial)
│   │   └── CH-01/                              # [COAFI-GPCOM-0300-AIC-01-GPC](#coafi-gpcom-0300-aic-01-gpc) (Capítulo de IA)
│   ├── QAO/                                    # [COAFI-GPCOM-0300-QAO-02-GPC](#coafi-gpcom-0300-qao-02-gpc) (Operaciones cuánticas avanzadas)
│   │   └── CH-02/                              # [COAFI-GPCOM-0300-QAO-02-GPC](#coafi-gpcom-0300-qao-02-gpc) (Capítulo de operaciones cuánticas)
│   └── docs/                                   # [COAFI-GPCOM-0000-DOC-00-GPC](#coafi-gpcom-0000-doc-00-gpc) (Documentación)
│
├── GP-RAME/                                    # [COAFI-GPRAME-0000-RAM-00-GPR](#coafi-gprame-0000-ram-00-gpr) (Gestión de recursos y materiales)
│   ├── README.md
│   ├── GEN/                                    # [COAFI-GPRAME-0600-GEN-00-GPR](#coafi-gprame-0600-gen-00-gpr) (General)
│   │   └── CH-00/                              # [COAFI-GPRAME-0600-GEN-00-GPR](#coafi-gprame-0600-gen-00-gpr) (Capítulo general)
│   ├── COMMON/                                 # [COAFI-GPRAME-0600-COM-10-GPR](#coafi-gprame-0600-com-10-gpr) (Recursos comunes)
│   │   └── CH-10/                              # [COAFI-GPRAME-0600-COM-10-GPR](#coafi-gprame-0600-com-10-gpr) (Capítulo de recursos comunes)
│   └── docs/                                   # [COAFI-GPRAME-0000-DOC-00-GPR](#coafi-gprame-0000-doc-00-gpr) (Documentación)
│
└── GP-SUPL/                                    # [COAFI-GPSUPL-0000-SUP-00-GPS](#coafi-gpsupl-0000-sup-00-gps) (Cadena de suministro)
    ├── README.md
    ├── GEN/                                    # [COAFI-GPSUPL-0500-GEN-00-GPS](#coafi-gpsupl-0500-gen-00-gps) (General)
    │   └── CH-00/                              # [COAFI-GPSUPL-0500-GEN-00-GPS](#coafi-gpsupl-0500-gen-00-gps) (Capítulo general)
    ├── ESRC/                                   # [COAFI-GPSUPL-0500-ESR-01-GPS](#coafi-gpsupl-0500-esr-01-gps) (Recursos sostenibles)
    │   └── CH-01/                              # [COAFI-GPSUPL-0500-ESR-01-GPS](#coafi-gpsupl-0500-esr-01-gps) (Capítulo de recursos sostenibles)
    └── docs/                                   # [COAFI-GPSUPL-0000-DOC-00-GPS](#coafi-gpsupl-0000-doc-00-gps) (Documentación)
```

## 9. GP-FD Structure

```plaintext
GP-FD/                                          # [COAFI-GPFD-0000-FND-00-GPF](#coafi-gpfd-0000-fnd-00-gpf) (Fundamentos y principios)
├── README.md
├── DEONTOLOGICAL-MANIFEST.md                   # [COAFI-GPFD-0000-DEM-00-GPF](#coafi-gpfd-0000-dem-00-gpf) (Manifiesto deontológico)
├── ATOC.md                                     # [COAFI-GPFD-0000-TOC-00-GPF](#coafi-gpfd-0000-toc-00-gpf) (Tabla de contenidos arquitectónica)
├── INFOCODE-REGISTRY.md                        # [COAFI-GPFD-0000-ICR-00-GPF](#coafi-gpfd-0000-icr-00-gpf) (Registro de infocódigos)
├── DEONTOLOGICAL-INTERFACES-CHARTER.md         # [COAFI-GPFD-0000-DIC-00-GPF](#coafi-gpfd-0000-dic-00-gpf) (Carta de interfaces deontológicas)
│
├── GEN/                                        # [COAFI-GPFD-0000-GEN-00-GPF](#coafi-gpfd-0000-gen-00-gpf) (General)
│   ├── CH-00/                                  # [COAFI-GPFD-0000-VIS-00-GPF](#coafi-gpfd-0000-vis-00-gpf) (Visión)
│   ├── CH-01/                                  # [COAFI-GPFD-0000-THR-01-GPF](#coafi-gpfd-0000-thr-01-gpf) (Teoría)
│   ├── CH-02/                                  # [COAFI-GPFD-0000-REG-02-GPF](#coafi-gpfd-0000-reg-02-gpf) (Regulación)
│   └── docs/                                   # [COAFI-GPFD-0000-DOC-00-GPF](#coafi-gpfd-0000-doc-00-gpf) (Documentación)
│
├── AMPIDE-SETUP.md                             # [COAFI-GPFD-0000-AMP-00-GPF](#coafi-gpfd-0000-amp-00-gpf) (Configuración de AMPIDE)
│
├── GAIA-CO-ASD-LIB/                            # [COAFI-GPFD-0000-GCL-00-GPF](#coafi-gpfd-0000-gcl-00-gpf) (Biblioteca GAIA-CO-ASD)
│   ├── file-formats/                           # [COAFI-GPFD-0000-FMT-00-GPF](#coafi-gpfd-0000-fmt-00-gpf) (Formatos de archivo)
│   ├── naming-convention/                      # [COAFI-GPFD-0000-NAM-00-GPF](#coafi-gpfd-0000-nam-00-gpf) (Convención de nomenclatura)
│   └── metadata/                               # [COAFI-GPFD-0000-MET-00-GPF](#coafi-gpfd-0000-met-00-gpf) (Metadatos)
│
└── docs/                                       # [COAFI-GPFD-0000-DOC-00-GPF](#coafi-gpfd-0000-doc-00-gpf) (Documentación)
    ├── AGIS/                                   # [COAFI-GPFD-0000-AGI-00-GPF](#coafi-gpfd-0000-agi-00-gpf) (Arquitectura GAIA de Sistemas Integrados)
    ├── TPSL-TPWD/                              # [COAFI-GPFD-0000-TPW-00-GPF](#coafi-gpfd-0000-tpw-00-gpf) (Teoría de Plataformas Sostenibles y Diseño de Plataformas Completas)
    ├── CFSI/                                   # [COAFI-GPFD-0000-CFS-00-GPF](#coafi-gpfd-0000-cfs-00-gpf) (Componentes Funcionales para Sistemas Integrados)
    ├── CEU/                                    # [COAFI-GPFD-0000-CEU-00-GPF](#coafi-gpfd-0000-ceu-00-gpf) (Componentes de Entidades Unificadas)
    ├── AGAD/                                   # [COAFI-GPFD-0000-AGA-00-GPF](#coafi-gpfd-0000-aga-00-gpf) (Arquitectura GAIA para Análisis de Datos)
    ├── URIF/                                   # [COAFI-GPFD-0000-URI-00-GPF](#coafi-gpfd-0000-uri-00-gpf) (Unidades de Referencia para Interfaces Federadas)
    └── e-GAIAs/                                # [COAFI-GPFD-0000-EGA-00-GPF](#coafi-gpfd-0000-ega-00-gpf) (Entidades GAIA Autónomas)
```

## 10. INFOCODE-INDEX

Los InfoCodes son subdirectorios estándar que se incluyen en cada componente para organizar la documentación y los artefactos según su tipo y propósito.

| InfoCode | Nombre | Descripción
|-----|-----|-----
| OV | Overview | Documentos de visión general y resúmenes ejecutivos
| SDD | System Design Description | Descripciones detalladas del diseño del sistema
| SPEC | Specifications | Especificaciones técnicas y requisitos
| TEST | Testing | Planes y procedimientos de prueba
| PROC | Procedures | Procedimientos operativos y de mantenimiento
| PLAN | Planning | Planes de programa y gestión
| IDX | Index | Índices y referencias cruzadas
| NEXUS | Interconnection Points | Puntos de interconexión federados entre componentes


## 11. GAIA-CO-ASD-LIB Standard

### 11.1 File Formats

| Formato | Extensión | Uso
|-----|-----|-----
| Markdown | .md | Documentación general, READMEs, guías
| JSON | .json | Configuración, datos estructurados
| YAML | .yaml, .yml | Configuración, definiciones de flujo de trabajo
| XML | .xml | Intercambio de datos estructurados
| CSV | .csv | Datos tabulares
| PDF | .pdf | Documentos formales, especificaciones finalizadas
| SVG | .svg | Gráficos vectoriales, diagramas
| PNG | .png | Imágenes, capturas de pantalla
| STEP | .step, .stp | Modelos CAD 3D
| GLTF | .gltf, .glb | Modelos 3D para visualización web
| TTL | .ttl | Ontologías y modelos semánticos (Turtle)
| OWL | .owl | Ontologías Web
| RDF | .rdf | Framework de descripción de recursos


### 11.2 Naming Convention

El formato general para nombres de archivo es:

```plaintext
COAFI-[DIVISION]-[CLASS]-[COMPONENT]-[NUMBER]-[TYPE]-[VERSION]-[STATUS].[EXT]
```

Donde:

- **DIVISION**: Código de división (ej., GPAM)
- **CLASS**: Identificador de clase (ej., 0100)
- **COMPONENT**: Código de componente de 3 letras (ej., ENG)
- **NUMBER**: Número de capítulo (ej., 72)
- **TYPE**: Tipo de documento (ej., SDD para System Design Description)
- **VERSION**: Número de versión (ej., v1-0-0)
- **STATUS**: Estado del documento (ej., DRAFT, APPROVED)
- **EXT**: Extensión del archivo (ej., md, json, pdf)


### 11.3 Metadata

Cada archivo debe incluir un bloque de metadatos en su encabezado con la siguiente información:

```yaml
---
title: "Título del documento"
coafi_code: "COAFI-GPAM-0100-ENG-72-SDD"
version: "1.0.0"
date: "2023-06-15"
status: "DRAFT"
authors: ["Autor 1", "Autor 2"]
reviewers: ["Revisor 1"]
approvers: ["Aprobador 1"]
tags: ["motor", "propulsión", "diseño"]
related_docs: ["COAFI-GPAM-0100-ENG-72-SPEC"]
abstract: "Breve descripción del contenido del documento"
---
```
