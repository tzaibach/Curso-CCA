![Cabecera PD Web OnePage QuickStart](_resources/heading.png "Cabecera PD Web OnePage QuickStart")

# Tabla de contenido 📇
1. [Información del producto](#1-información-del-producto-)
2. [Especificaciones Técnicas](#2-especificaciones-técnicas-)
3. [Pruebas](#3-pruebas-)


----------

# 1. Información del producto 📦

* Nombre del Servicio: **pd-web-MODIFICAR** 🚧
* Fecha de publicación: **Fecha prevista de publicación o fecha de publicación** 🚧
* URL:
  * PRO → https://www.juntadeandalucia.es/MODIFICAR ó https://www.MODIFICAR.es/ 🚧
  * DES → https://desarrollo.juntadeandalucia.es/MODIFICAR ó https://MODIFICAR.junta-andalucia.es/ 🚧

* Responsable/s Funcional: 
  * **MODIFICAR 1** (Organismo / Centro Directivo) 🚧
  * **MODIFICAR 2** (Organismo / Centro Directivo) 🚧

* Responsable/s Técnico:
  * **MODIFICAR 1** (Organismo / Centro Directivo) 🚧
  * **MODIFICAR 2** (Organismo / Centro Directivo) 🚧

* Información adicional:
  * Si el producto es de organismos externos, solicitar certificado (Bloqueado paso a producción hasta su recepción)
  * Si el solicitante es CPAI, crear ticket relacionado para su gestión.

## 1.1 Descripción Funcional

Texto Descriptivo del sitio web, principales secciones, objetivos, etc ... 🚧

# 2. Especificaciones Técnicas 👷

## 2.1 Descripción Técnica

Se trata de un producto digital de tipo OnePage, esto implica que tiene una página estática y no realiza peticiones a ningún servicio backend. Este tipo de servicios están clonados a raíz de un proyecto base alojado en el siguiente repositorio: https://gitlab.juntadeandalucia.es/pd-web-templates/pd-web-onepage-quickstart.</p

## 2.2. Datos Técnicos

* Plantilla Base : https://gitlab.juntadeandalucia.es/pd-web-templates/pd-web-onepage-quickstart.
* Estrategia de despliegue: <br>El despliegue del servicio está basado en la integración continua. Mediante un webhook se enlaza el repositorio del código fuente con la aplicación de Openshift. Cuando el repositorio es actualizado, se manda una señal mediante el webhook al build de la aplicación. Este realiza un build con la nueva información y lo aloja en la imagen de Openshift que automáticamente es desplegada por el deployment.<br>
Para mayor información del proceso automatizado de despliegue ver [Proceso despliegue OPS](https://gitlab.juntadeandalucia.es/pd-web-templates/pd-web-onepage-quickstart/wikis/home#02-creaci%C3%B3n-pd-web-onepage-en-openshift "Proceso despliegue OPS")
  * Enlace de OpenShift en desarrollo:https://openshift-des.sandetel.junta-andalucia.es:8443/console/project/MODIFICAR/overview 🚧
  * Enlace de OpenShift en producción:https://paas.junta-andalucia.es:8443/console/project/MODIFICAR/overview 🚧

* Monitorización: **12x5 - Soporte en horario de oficina** / **24x7 Crítico** / **24x7 Servicio** 🚧
En caso de ser 24x7 es necesario contacto telefónico con responsable técnico para aviso.

* Disponibilidad del Servicio:
  * Readiness Probe: GET / on port 8080 (HTTP) 3s delay, 1s timeout
  * Liveness Probe: GET / on port 8080 (HTTP) 3s delay, 1s timeout
* Recursos
  * Número de unidades proceso (mcores): 150 mcores (limit) y 75 mcores (request)
  * Memoría asignada: 50 MiB (limit) y 25 MiB (request)
  * Almacenamiento: Al tratarse de un servicio OnePage **no requiere de volumen de almacenamiento**
* Routes
  * PRO → https://MODIFICAR.paas.junta-andalucia.es 🚧
  * DES → https://MODIFICAR.apps-des.sandetel.junta-andalucia.es 🚧
* Backup: No es necesario, el despliegue se realiza de forma completa desde GitLab
* Autoescalado: No

# 3. Pruebas 🧪 

## 3.1. Pruebas Automáticas

Pruebas de carga: Onepage.jmx
Resultados pruebas de carga: Onepage.jtl

## 3.2. Pruebas Funcionales

* Pruebas funcionales: Plan_de_pruebas_onepage.xlsx
* Comprobar que el sitio es navegable con la url del entorno
* Comprobar los enlaces de la página si son correctos (Pendiente definición final de enlaces)
* Pruebas particulares de éste sitio 🚧

## 3.3. Pruebas de Accesibilidad

Pruebas de accesibilidad: Test_de_accesibilidad.odt

## 3.4. Pruebas de despliegue

Comprobación de páginas publicadas
