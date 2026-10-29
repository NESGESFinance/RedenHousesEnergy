# RedenHousesEnergy: Ecosistema de Energía Circular & Tokenización RWA sobre Bitcoin

**Repositorio Oficial de Ingeniería, Arquitectura Ciberfísica y Modelado Financiero de RedenHousesEnergy (RHE 2026-2030)**  
*Desarrollado y promovido por **NESGESFinance Ecosystem S.A.S. BIC** (Ecuador) & **NESGESFinance Ecosystem S.A.S. LLC** (New Mexico, EE. UU. #0008086872).*  
*Liderazgo del Proyecto: **Cbr. Joan Santiago Ramírez Almeida** (CEO-Founder NESGESFinance / @RedenHousesGlobal).*

---

## Tabla de Contenidos

1. [Visión General del Proyecto](#visión-general-del-proyecto)
2. [Especificaciones y Métricas Clave](#especificaciones-y-métricas-clave)
3. [Arquitectura Ciberfísica: Las 6 Eco-Tecnologías y Capa BESS v2.0](#arquitectura-ciberfísica-las-6-eco-tecnologías-y-capa-bess-v20)
   - [1. Torre de Sales Fundidas (Núcleo Térmico)](#1-torre-de-sales-fundidas-núcleo-térmico)
   - [2. Campo Fotovoltaico Concéntrico (72 MWp)](#2-campo-fotovoltaico-concéntrico-72-mwp)
   - [3. Almacenamiento Gravitacional Subterráneo](#3-almacenamiento-gravitacional-subterráneo)
   - [4. Motores Brushless (BLDC) de Precisión](#4-motores-brushless-bldc-de-precisión)
   - [5. Planta de Pirólisis Inversa](#5-planta-de-pirólisis-inversa)
   - [6. Turbinas Termoeléctricas (Vapor y Gas)](#6-turbinas-termoeléctricas-vapor-y-gas)
   - [7. Capa BESS LiFePO4 de Estabilización Fina (Versión 2.0)](#7-capa-bess-lifepo4-de-estabilización-fina-versión-20)
4. [Sistema de Control SCADA, IoT Edge y Oráculos Criptográficos](#sistema-de-control-scada-iot-edge-y-oráculos-criptográficos)
5. [Modelo de Tokenización RWA sobre Bitcoin (L1 y L2)](#modelo-de-tokenización-rwa-sobre-bitcoin-l1-y-l2)
6. [Estructuración Financiera, DCF y Modelo WACC](#estructuración-financiera-dcf-y-modelo-wacc)
   - [Matriz de CAPEX Mínimo y Medio](#matriz-de-capex-mínimo-y-medio)
   - [Estructura de OPEX y Capital](#estructura-de-opex-y-capital)
   - [Formulación Matemática y WACC](#formulación-matemática-y-wacc)
   - [Matriz de 6 Flujos de Ingreso Diversificados](#matriz-de-6-flujos-de-ingreso-diversificados)
7. [Marco Legal BIC, Gobernanza Bicontinental y Estructura SPV](#marco-legal-bic-gobernanza-bicontinental-y-estructura-spv)
8. [Matriz de Riesgos y Plan de Mitigación (Auditoría AUD-NESGES-2026-RHE-001)](#matriz-de-riesgos-y-plan-de-mitigación-auditoría-aud-nesges-2026-rhe-001)
9. [Estructura del Repositorio y Archivos](#estructura-del-repositorio-y-archivos)
10. [Hoja de Ruta de Ejecución (Roadmap 2026-2030)](#hoja-de-ruta-de-ejecución-roadmap-2026-2030)
11. [Aviso Legal, Compliance y Licencia](#aviso-legal-compliance-y-licencia)

---

## Visión General del Proyecto

**RedenHousesEnergy (RHE)** es un megaproyecto de infraestructura ciberfísica de energía circular diseñado para eliminar de manera estructural la intermitencia inherente a las fuentes renovables variables. Ubicado en un predio de **90 hectáreas en el cantón Ibarra, sector Salinas, provincia de Imbabura, Ecuador (latitud 00° N)**, el complejo integra seis tecnologías limpias complementarias más una capa de almacenamiento electroquímico ultravanzado.

A diferencia de las centrales termoeléctricas tradicionales o represas hidroeléctricas que consumen millones de metros cúbicos de agua o alteran los cauces fluviales, RHE funciona bajo un **circuito cerrado aerotérmico de condensación** que evita la extracción de agua de ríos o acuíferos locales (recuperación del 99,8% del agua de proceso). El proyecto satisface las necesidades energéticas de su propio parque industrial y comercializa excedentes netos a la red pública gestionada por la Empresa Eléctrica Regional Norte (CNEL EP) bajo contratos PPA de largo plazo.

---

## Especificaciones y Métricas Clave

| Parámetro Técnico / Financiero | Valor Nominal / Rango de Diseño | Observación / Referencia de Ingeniería |
| :--- | :--- | :--- |
| **Ubicación Geográfica** | Cantón Ibarra, Imbabura, Ecuador | Latitud ecuatorial 00° N (GHI: $4,5 - 5,5 \text{ kWh/m}^2/\text{día}$) |
| **Superficie del Predio** | 90 hectáreas ($900.000 \text{ m}^2$) | Predio industrial y de generación fotovoltaica concéntrica |
| **Potencia Fotovoltaica Instalada** | 72 MWp nominal (70-75 MWp) | Módulos monocristalinos TOPCon bifaciales de alta eficiencia |
| **Reserva Térmica Directa** | 15 horas a plena carga | Batería térmica de Solar Salt (300 °C - 600 °C) |
| **Disponibilidad Operativa** | $> 98,5\%$ ($24/7/365$) | Suministro ininterrumpido sin dependencia meteorológica |
| **Producción Bruta Estimada** | $144,5 \text{ GWh/año}$ ($\\approx 396 \text{ MWh/día}$) | Inyección neta a red estimada en $130 - 140 \text{ GWh/año}$ |
| **Cobertura Equivalente** | $40.000 - 50.000 \text{ hogares}$ | Abastecimiento continuo para consumo residencial e industrial |
| **Presupuesto CAPEX Mínimo / Medio**| $\$118 \text{ M USD} - \$158 \text{ M USD}$ | Techo de inversión estimado en $\$198 \text{ M USD}$ |
| **Costo Operativo Anual (OPEX)** | $\$4,7 \text{ M USD/año}$ | $\\approx 2,8\%$ del CAPEX medio con mantenimiento predictivo |
| **Periodo de Retorno (Payback)** | $12 - 16 \text{ años}$ | Con ingresos diversificados ($19 - 24 \text{ años}$ solo PPA) |
| **Vida Útil de Infraestructura** | $> 30 \text{ años}$ | Diseño mecánico y térmico con redundancia industrial |

---

## Arquitectura Ciberfísica: Las 6 Eco-Tecnologías y Capa BESS v2.0

### 1. Torre de Sales Fundidas (Núcleo Térmico)
* **Composición del Fluido:** Mezcla inorgánica binaria *Solar Salt* ($60\% \text{ NaNO}_3 / 40\% \text{ KNO}_3$).
* **Rango Térmico de Operación:** Fluidización de 300 °C a 600 °C (punto óptimo de transferencia en receptor a 565 °C).
* **Densidad Energética:** $\\approx 350 \text{ kWh/m}^3$ con capacidad para proporcionar hasta **15 horas de reserva térmica continua**.
* **Protección Anti-Solidificación (*Heat-Tracing*):** Para evitar la congelación irreversible de las sales a 220 °C, el sistema cuenta con un circuito de trazado eléctrico asistido por gas sintético y control predictivo 24/7, manteniendo la temperatura de reserva siempre por encima de los 250 °C.
* **Insumos Locales:** Construcción reforzada utilizando sal marina procesada de la costa ecuatoriana y ceniza volcánica puzolánica andina para aislamiento y resistencia estructural.

### 2. Campo Fotovoltaico Concéntrico (72 MWp)
* **Diseño Híbrido:** Arreglos dispuestos en anillos concéntricos alrededor de la torre central. Un subconjunto opera como helióstatos reflejantes y el resto como campo fotovoltaico directo con celdas TOPCon bifaciales (eficiencia $22\% - 24\%$).
* **Seguimiento Automatizado:** Seguidores solares (*trackers*) de dos ejes controlados por algoritmos de inteligencia artificial edge que ejecutan ajustes de inclinación en tiempo real para eliminar sombreado mutuo (*backtracking*).

### 3. Almacenamiento Gravitacional Subterráneo
* **Infraestructura:** **4 pozos subterráneos verticales de 100 metros de profundidad** y 1,5 metros de radio interno, con recubrimiento de polímeros sintéticos de ultra baja fricción y estructura sismo-resistente.
* **Principio Físico:** Almacena energía potencial gravitacional ($E = m \cdot g \cdot h$) mediante la elevación de masas sólidas de alta densidad durante superávits solares. Al liberarse en caída controlada, reinyecta energía a la red con tiempos de respuesta **inferiores a 100 milisegundos**.

### 4. Motores Brushless (BLDC) de Precisión
* **Control Electromecánico:** Instalados en la cabezal de superficie de los pozos gravitacionales, operan con control vectorial reversible.
* **Regeneración de Potencia:** Regulan el descenso de los pesos con precisión electrónica para mantener la estabilidad de frecuencia en la microred y conmutan a modo motor de alta eficiencia para la fase de recarga.

### 5. Planta de Pirólisis Inversa
* **Capacidad de Procesamiento:** 15 a 25 toneladas diarias de residuos plásticos posconsumo (polietileno PE y polipropileno PP, excluyendo PVC).
* **Descomposición Térmica:** Pirólisis anaeróbica a $400 \text{ °C} - 500 \text{ °C}$ para obtener aceite pirolítico sintético (rendimiento $60\% - 80\%$ comercializable a $\$0,70 - \$0,90 \text{ USD/L}$), gas síntesis (*syngas* metano/propano) y biochar sólido.
* **Respaldo Térmico:** El *syngas* alimenta turbinas de gas de arranque rápido ($< 12 \text{ min}$), sirviendo como salvaguarda frente a períodos prolongados de alta nubosidad.

### 6. Turbinas Termoeléctricas (Vapor y Gas)
* **Ciclo Rankine:** Turbina de vapor de alta presión acoplada al intercambiador de calor de sales fundidas con eficiencia térmica del $41\% - 43\%$.
* **Ciclo de Gas:** Turbinas de gas secundarias alimentadas por *syngas* para absorber picos súbitos de consumo o suplir carga base durante mantenimientos programados.

### 7. Capa BESS LiFePO4 de Estabilización Fina (Versión 2.0)
* **Capacidad e Integración:** Banco de Baterías de Litio-Ferrofosfato ($\text{LiFePO}_4$) de **8 a 12 MWh de capacidad y 4 a 6 MW de potencia**.
* **Gestión Dinámica de Carga:** Controlado por BMS inteligente con **límite dinámico de profundidad de descarga (DoD) máximo del 80%** (SOC operativo de 20% a 90%). Esta salvaguarda preserva el electrodo y extiende la durabilidad del banco a **6.000-8.000 ciclos útiles (10 a 12 años)**.

---

## Sistema de Control SCADA, IoT Edge y Oráculos Criptográficos

El sistema operativo de RedenHousesEnergy implementa una arquitectura distribuida **Edge-Fog-Cloud** que conecta la infraestructura industrial con la blockchain de Bitcoin:

1. **Nivel 1: IoT Edge**: Medidores inteligentes equipados con HSM (*Hardware Security Module*) y sensores distribuidos en la torre térmicas, pozos gravitacionales, banco BESS, planta de pirólisis e inversores fotovoltaicos.
2. **Nivel 2: Fog & SCADA**: Controladores Lógicos Programables (PLC) industriales, gemelo digital (*Digital Twin*) y despacho estocástico basado en machine learning.
3. **Nivel 3: Oráculos Web3**: Red de oráculos multifuente (Chainlink + oráculo propio firmado desde HSM) para la verificación física de kilovatios-hora generados y la emisión de Certificados de Producción CP-NGF.
4. **Nivel 4: Bitcoin Blockchain**: Registro en Capa 1 (Bitcoin Runes y Ordinals UTXO) y liquidación automatizada en Capa 2 (Lightning Network).

---

## ₿ Modelo de Tokenización RWA sobre Bitcoin (L1 y L2)

RedenHousesEnergy ancla su arquitectura financiera digital de Activos del Mundo Real (RWA) exclusivamente sobre la red **Bitcoin**:

### Capa 1: Bitcoin Mainnet (Propiedad e Infraestructura)
1. **Utility Token (`$NGF` / `NGF•BTC•AM`):**
   - Emitido bajo el protocolo **Bitcoin Runes**.
   - Suministro fijo e inalterable: **5.930.000.000 unidades**.
   - **Funcionalidad:** Permite acceso al ecosistema, micro-tarifación de servicios energéticos, peajes en la microred y gobernanza interna. *No otorga derechos a dividendos ni participación accionaria*.
2. **Security Tokens (`NGF-RHE-BTC`):**
   - Estructurados mediante **Project Ordinals (UTXO)** en Bitcoin L1.
   - **Funcionalidad:** Representan títulos fraccionados de propiedad sobre la SPV, derechos sobre el flujo de caja neto y voto en decisiones corporativas clave.

### Capa 2: Lightning Network (Liquidación y Rendimientos)
* **Liquidación de Micropagos:** El motor SCADA valida la producción física diaria ($kWh$, litros de aceite, $t \text{ CO}_2$). Tras descontar costos operativos (OPEX) y la cuota del fondo de reserva, convierte los flujos netos a satoshis y distribuye micropagos periódicos directamente a las billeteras Taproot de los inversores.
* **Proof of Reserve (PoR) 1:1:** Un contrato audita automáticamente en cadena cada 6 horas que el $100\%$ de los tokens emitidos cuenten con respaldo de activos físicos y reservas bancarias 1:1.
* **Fondo de Reserva de Liquidez:** Se establece una reserva obligatoria equivalente al **10% del CAPEX total** en el *Liquidity Pool* para proteger el ecosistema contra volatilidad en stablecoins o brechas temporales de iliquidez.

---

## Estructuración Financiera, DCF y Modelo WACC

### Matriz de CAPEX Mínimo y Medio

| Componente de Infraestructura | Presupuesto Mínimo (USD) | Presupuesto Medio (USD) | Participación (%) |
| :--- | :---: | :---: | :---: |
| **Sistema Fotovoltaico (72 MWp)** | $\$50 \text{ M}$ | $\$60 \text{ M}$ | $38,0\%$ |
| **Obras Civiles, Subestación e Ingeniería FEED** | $\$27 \text{ M}$ | $\$32 \text{ M}$ | $20,3\%$ |
| **Torre de Sales Fundidas (Núcleo Térmico)** | $\$15 \text{ M}$ | $\$20 \text{ M}$ | $12,7\%$ |
| **Pozos Gravitacionales y Motores Brushless** | $\$13 \text{ M}$ | $\$15 \text{ M}$ | $9,5\%$ |
| **Planta de Pirólisis Inversa y Turbinas** | $\$13 \text{ M}$ | $\$18 \text{ M}$ | $11,4\%$ |
| **Capa BESS LiFePO4 y Control SCADA** | $\$5 \text{ M}$ | $\$8 \text{ M}$ | $5,1\%$ |
| **TOTAL CAPEX PROYECTADO** | **$\$118 \text{ M}$** | **$\$158 \text{ M}$** | **$100,0\%$** |

### Estructura de OPEX y Capital
* **Costo Operativo Anual (OPEX):** $\$4,7 \text{ M USD/año}$ ($\\approx 2,8\% - 3,0\%$ del CAPEX de referencia).
* **Estructura de Financiación Objetivo:** $55\% - 65\%$ Equity / Tokens RWA y $35\% - 45\%$ Deuda Verde / Crédito Institucional.

### Formulación Matemática y WACC

El Costo Promedio Ponderado de Capital ($WACC$) incorpora las primas de riesgo país (Ecuador) y riesgo tecnológico/cripto:

$$WACC = \left( \frac{E}{V} \cdot K_e \right) + \left( \frac{D}{V} \cdot K_d \cdot (1 - t) \right)$$

Donde:
* $E$: Capital equity de tokens e inversores.
* $D$: Deuda financiera o créditos verdes.
* $V = E + D$: Capital total de la SPV.
* $K_e$: Costo del capital propio con prima RWA/cripto de $+450 \text{ a } +650 \text{ pb}$ ($K_e \approx 14\% - 16\%$).
* $K_d$: Costo de la deuda corporativa ($K_d \approx 7,5\% - 9,0\%$).
* $t$: Tasa impositiva corporativa aplicable en Ecuador.

Fórmula de ingreso anual indexado a la inflación del sector eléctrico regulado ($\pi$):

$$Ingreso_t = E_{generada, t} \times \left[ Tarifa_{base} \times (1 + \pi)^t \right] - OPEX_t + Valor_{RWA, t}$$

### Matriz de 6 Flujos de Ingreso Diversificados

1. **Venta de Energía (PPA CNEL EP) [55%]:** Comercialización de $130 - 140 \text{ GWh/año}$ netos a tarifa PPA de $\$0,09 - \$0,12 \text{ USD/kWh}$.
2. **Aceite Pirolítico Sintético [12%]:** Venta de combustible pirolítico a $\$0,70 - \$0,90 \text{ USD/litro}$.
3. **Bonos de Carbono Verra VM0042 [10%]:** Mitigación certificada comercializada a $\$15 - \$50 \text{ USD/t CO}_2\text{eq}$.
4. **Estabilización de Red [10%]:** Servicios auxiliares de regulación de frecuencia y *peak shaving* con respuesta gravitacional $<100 \text{ ms}$.
5. **Certificados CP-NGF [7%]:** Venta de atributos renovables y origen verde con trazabilidad en blockchain.
6. **Biochar Agrícola [6%]:** Venta de carbono residual para acondicionamiento y regeneración de suelos agrícolas.

---

## Marco Legal BIC, Gobernanza Bicontinental y Estructura SPV

Para lograr el aislamiento de riesgos pasivos y activos (*ring-fencing*), el proyecto opera a través de tres entidades jurídicas:

1. **`NESGESFinance Ecosystem S.A.S. BIC` (Ibarra, Ecuador):** Operador local encargada del desarrollo en el predio de 90 ha, licenciamiento ambiental TULSMA Categoría IV / EIA y trámites de conexión PPA ante ARCONEL y CNEL EP.
2. **`NESGESFinance Ecosystem S.A.S. LLC` (New Mexico, EE. UU. #0008086872):** Custodia de propiedad intelectual, cumplimiento *compliance* internacional y estructuración de capital bajo SEC Reg D Rule 506(c) para inversores acreditados.
3. **`RedenHousesEnergy SPV01 LLC` (Vehículo SPV Aislado):** Titularidad exclusiva de los activos físicos del parque de Ibarra, emisión de Security Tokens (`NGF-RHE-BTC`) y segregación de flujos de caja.

---

## Matriz de Riesgos y Plan de Mitigación (Auditoría AUD-NESGES-2026-RHE-001)

| Categoría | Riesgo Identificado | Impacto (1-5) | Prob. (1-5) | Estrategia de Mitigación Obligatoria |
| :--- | :--- | :---: | :---: | :--- |
| **Técnico** | Solidificación de sales por caída térmicas ($< 220 \text{ °C}$) | 5 | 3 | Sistema de *heat-tracing* alimentado por gas y control SCADA 24/7. |
| **Técnico** | Degradación acelerada del banco BESS $\text{LiFePO}_4$ | 4 | 2 | Restricción estricta de DoD máximo al 80% (SOC 20%–90%) vía BMS. |
| **Técnico** | Falla en protecciones anti-isla en la microred | 5 | 2 | Certificación y cumplimiento de normas IEEE 1547 e IEC 62116. |
| **Financiero** | Mismatch de liquidez en stablecoins / tokens RWA | 4 | 3 | Fondo de reserva de liquidez $\ge 10\%$ del CAPEX + PoR 1:1 on-chain. |
| **Regulatorio** | Modificaciones en esquemas de Net Metering / PPA | 5 | 3 | Diversificación hacia servicios auxiliares de red y venta de aceite. |
| **Legal / Cripto**| Clasificación de tokens como *securities* no registrados | 5 | 4 | Opinión legal dual (Ecuador y SEC Reg D 506(c) en EE. UU.) pre-emisión. |
| **Ciberseguridad**| Ataque Man-in-the-Middle a medidores o SCADA | 5 | 2 | Red OT aislada, chips HSM en medidores y oráculos multifuente. |

---

## Estructura del Repositorio y Archivos

El presente repositorio reúne la documentación técnica, legal, financiera y las simulaciones del ecosistema:

* `README.md`: Documentación principal del repositorio.
* `InformeTecnico_Empresarial_2026 RedenHousesEnergy.pdf`: Dossier técnico-empresarial completo (2026).
* `RedenHousesEnergy_Descripción_Completa.pdf`: Ensayo técnico integrado y plan maestro.
* `DOC-20261028-WA0026.pdf`: Expediente de auditoría senior por pares.
* `RedenHousesEnergy Whitepaper.pdf`: Whitepaper oficial de tokenización RWA.
* `RedenHousesEnergy Integración de Tecnologías.pdf`: Manual de ingeniería y acoplamiento de sistemas.
* `Graficas_RedenHousesEnergy.pdf`: Esquemas termodinámicos y diagramas de flujo.
* `Dashboard_RedenHousesEnergy_19_07 (1).html`: Dashboard interactivo en HTML/JS.
* `dashboard_completo_redenhousesenergy_v3.pdf`: Reporte gráfico de indicadores y KPIs.
* `Informe Técnico y Auditoría Senior.md`: Informe técnico en formato Markdown.
* `IMG-20261014-WA0015.jpg` ... `WA0028.jpg`: Renderizados 3D, mapas y diagramas de predio.
* `RedenHousesEnergy.jpg`: Infografía principal del ecosistema.

---

## Hoja de Ruta de Ejecución (Roadmap 2026-2030)

1. **Q4 2026 – Q1 2027**: Ingeniería de Detalle (FEED), Estudio Geotécnico/Sísmico, EIA Cat. IV y Dictamen Legal.
2. **Q2 2027 – Q3 2027**: Estructuración Financiera, Auditoría de Smart Contracts L2, Fondo de Reserva 10%.
3. **Q4 2027 – FY 2028**: Construcción Fase Piloto (Torre parcial, 2 Pozos Gravitacionales, 20 MWp FV, BESS 4 MWh).
4. **FY 2029**: Interconexión Nacional (CNEL EP PPA), Operación Comercial e Inicio Dividendos L2.
5. **FY 2030**: Capacidad Nominal Completa (72 MWp, 4 Pozos, Pirólisis plena -> $144,5 \text{ GWh/año}$).

---

## Aviso Legal, Compliance y Licencia

### Descargo de Responsabilidad (*Disclaimer*)
1. **Carácter Informativo:** Las cifras, capacidades, costos y retornos presentados en este repositorio constituyen proyecciones de ingeniería y modelos financieros sujetos a verificación en la fase FEED y estudios de impacto ambiental. No representan un folleto de emisión ni una garantía de rendimiento.
2. **Cumplimiento de Valores (*Securities*):** Ningún token descrito en este proyecto constituye una oferta pública de valores no registrados. La eventual comercialización de Security Tokens se realizará bajo exenciones aplicables como la Regulación D Regla 506(c) de la SEC en Estados Unidos para inversores acreditados.
https://RedenHousesEnergy.org
https://NESGESFinance.org
3. **Derechos Reservados:** © 2025-2026 **NESGESFinance Ecosystem S.A.S. BIC** & **NESGESFinance Ecosystem S.A.S. LLC**. Todos los derechos reservados.

---

<p align="center">
  <b>NESGESFinance Ecosystem S.A.S. BIC</b> • Cantón Ibarra, Imbabura, Ecuador (00° N)<br>
  <i>Infraestructura para un nuevo ciclo energético: De la energía continua a Bitcoin.</i>
</p>