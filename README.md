# Asesor de protecciones REBT

Versión beta 1 (11-10-2026). Los cambios de cada versión están en [CAMBIOS.md](CAMBIOS.md).

Indica qué protecciones poner en cada cuadro de una instalación eléctrica de baja tensión nueva, según el REBT: interruptor general, protector contra sobretensiones, diferenciales y curva de los magnetotérmicos. Es una sola página (`index.html`) que funciona en el navegador, sin instalar nada, y está pensada para usarse también desde el móvil.

Es hermana de la [Calculadora REBT](https://east101.github.io/calculadora-rebt/), que calcula secciones, caídas de tensión y calibres.

## Qué instalaciones cubre

- Vivienda: cuadro general y subcuadros en paralelo, cada uno con su diferencial de 30 mA (ITC-BT-25)
- Local o terciario: árbol de cuadros con diferenciales en serie y selectivos
- Industria: lo mismo, con 300 mA permitidos en receptores fijos y tipo AC donde no hay electrónica

Solo esquema TT.

## Qué indica

- Diferenciales de cada cuadro: sensibilidad, retardo, tipo (AC, A, F o B) y cuántos hacen falta
- Cascada de selectividad de hasta cuatro niveles, con gráfica de tiempos y veredicto
- Curva de los magnetotérmicos (C o D) según los receptores
- En vivienda: interruptor general (25 o 40 A), poder de corte mínimo y calibre de cada circuito
- Protector contra sobretensiones: si es obligatorio o recomendado, de qué tipo y dónde va
- Estimación de fugas permanentes bajo cada diferencial
- Resistencia de tierra máxima
- Cada dato con su motivo y su cita, marcado como obligatorio, recomendado, previsto o criterio técnico
- Esquema descargable como imagen y resumen en texto para copiar

## Fuentes

- REBT, texto consolidado del BOE a 3-9-2025: ITC-BT-10, 17, 18, 23, 24, 25 y 52
- Guías técnicas de aplicación BT-18, BT-22, BT-23, BT-24, BT-25 y BT-26
- UNE-HD 60364-4-41, ap. 411.3.2 (tiempos máximos de corte)
- Manual de protección diferencial de APIEM (2022): fugas típicas, tipos y selectividad
- Catálogos de fabricante: Hager (tiempos de diferenciales), Schneider Acti9 (curvas) y ComPacT NSX (retardos y tiempos de corte de la protección diferencial regulable)
- Proyecto de modificación del REBT (presentación de COGITI): se cita como "previsto", no está en vigor

## Criterios propios

No salen del reglamento y se marcan en la app como "criterio técnico":

- Curva C como mínimo en todos los casos
- 300 mA para receptores fijos en industria, 30 mA en local
- Cabecera de 300 mA sobre 30 mA, en lugar de 100 mA
- Qué receptores se consideran "equipos sensibles" para recomendar protector contra sobretensiones

## Licencia

Creative Commons BY-NC-SA 4.0: se puede usar y adaptar citando la autoría, sin fines comerciales y compartiendo con la misma licencia.

## Aviso

Orientativo. No sustituye al proyecto ni a la memoria técnica. Los tiempos de los diferenciales regulables son los de un fabricante concreto: con otro, hay que comprobar su tabla.

