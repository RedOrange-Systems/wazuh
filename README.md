# Wazuh

[![Slack](https://img.shields.io/badge/slack-join-blue.svg)](https://wazuh.com/community/join-us-on-slack/)
[![Email](https://img.shields.io/badge/email-join-blue.svg)](https://groups.google.com/forum/#!forum/wazuh)
[![Documentation](https://img.shields.io/badge/docs-view-green.svg)](https://documentation.wazuh.com)
[![Documentation](https://img.shields.io/badge/web-view-green.svg)](https://wazuh.com)
[![Coverity](https://scan.coverity.com/projects/10992/badge.svg)](https://scan.coverity.com/projects/wazuh-wazuh)
[![Twitter](https://img.shields.io/twitter/follow/wazuh?style=social)](https://twitter.com/wazuh)
[![YouTube](https://img.shields.io/youtube/views/peTSzcAueEc?style=social)](https://www.youtube.com/watch?v=peTSzcAueEc)


Wazuh es una plataforma gratuita y de código abierto utilizada para la prevención, detección y respuesta ante amenazas. Es capaz de proteger cargas de trabajo en entornos locales, virtualizados, en contenedores y basados en la nube.

La solución Wazuh consta de un agente de seguridad para endpoints, desplegado en los sistemas monitorizados, y un servidor de gestión, que recopila y analiza los datos recogidos por los agentes. Además, Wazuh se ha integrado completamente con Elastic Stack, proporcionando un motor de búsqueda y una herramienta de visualización de datos que permite a los usuarios navegar por sus alertas de seguridad.

## Capacidades de Wazuh

Una breve presentación de algunos de los casos de uso más comunes de la solución Wazuh.

**Detección de intrusiones**

Los agentes de Wazuh escanean los sistemas monitorizados en busca de malware, rootkits y anomalías sospechosas. Pueden detectar archivos ocultos, procesos encubiertos o escuchas de red no registradas, así como incoherencias en las respuestas a las llamadas al sistema.

Además de las capacidades del agente, el componente de servidor utiliza un enfoque basado en firmas para la detección de intrusiones, empleando su motor de expresiones regulares para analizar los datos de registro recopilados y buscar indicadores de compromiso.

**Análisis de datos de registro (logs)**

Los agentes de Wazuh leen los registros del sistema operativo y de las aplicaciones, y los reenvían de forma segura a un gestor central para su análisis basado en reglas y su almacenamiento. Cuando no hay ningún agente desplegado, el servidor también puede recibir datos mediante syslog desde dispositivos de red o aplicaciones.

Las reglas de Wazuh te ayudan a detectar errores de aplicaciones o del sistema, configuraciones incorrectas, actividades maliciosas intentadas y/o exitosas, violaciones de políticas y otros diversos problemas de seguridad y operativos.

**Monitorización de la integridad de archivos**

Wazuh monitoriza el sistema de archivos, identificando cambios en el contenido, permisos, propiedad y atributos de los archivos que necesitas vigilar. Además, identifica de forma nativa los usuarios y aplicaciones utilizados para crear o modificar archivos.

Las capacidades de monitorización de la integridad de archivos pueden usarse en combinación con inteligencia de amenazas para identificar amenazas o hosts comprometidos. Además, varios estándares de cumplimiento normativo, como PCI DSS, lo requieren.

**Detección de vulnerabilidades**

Los agentes de Wazuh extraen datos del inventario de software y envían esta información al servidor, donde se correlaciona con bases de datos de CVE (Common Vulnerabilities and Exposure) actualizadas continuamente, con el fin de identificar software vulnerable conocido.

La evaluación automatizada de vulnerabilidades te ayuda a encontrar los puntos débiles en tus activos críticos y a tomar medidas correctivas antes de que los atacantes los exploten para sabotear tu negocio o robar datos confidenciales.

**Evaluación de la configuración**

Wazuh monitoriza la configuración del sistema y de las aplicaciones para asegurarse de que cumplen con tus políticas de seguridad, estándares y/o guías de hardening. Los agentes realizan escaneos periódicos para detectar aplicaciones conocidas por ser vulnerables, sin parchear o configuradas de forma insegura.

Además, las comprobaciones de configuración pueden personalizarse, adaptándolas correctamente a tu organización. Las alertas incluyen recomendaciones para una mejor configuración, referencias y correspondencia con el cumplimiento normativo.

**Respuesta a incidentes**

Los agentes de Wazuh proporcionan respuestas activas listas para usar, para llevar a cabo diversas contramedidas y hacer frente a amenazas activas, como bloquear el acceso a un sistema desde la fuente de la amenaza cuando se cumplen ciertos criterios.

Además, Wazuh puede utilizarse para ejecutar de forma remota comandos o consultas del sistema en los agentes, identificando indicadores de compromiso (IOC) y ayudando a realizar otras tareas de análisis forense en vivo o respuesta a incidentes.

**Cumplimiento normativo**

Wazuh proporciona algunos de los controles de seguridad necesarios para cumplir con estándares y regulaciones de la industria. Estas características, combinadas con su escalabilidad y soporte multiplataforma, ayudan a las organizaciones a cumplir con los requisitos técnicos de cumplimiento.

Wazuh es ampliamente utilizado por empresas de procesamiento de pagos e instituciones financieras para cumplir con los requisitos de PCI DSS (Payment Card Industry Data Security Standard). Su interfaz de usuario web ofrece informes y paneles de control que pueden ayudar con esta y otras regulaciones (por ejemplo, GPG13 o GDPR).

**Seguridad en la nube**

Wazuh ayuda a monitorizar la infraestructura en la nube a nivel de API, utilizando módulos de integración capaces de extraer datos de seguridad de proveedores de nube conocidos, como Amazon AWS, Azure o Google Cloud. Además, Wazuh proporciona reglas para evaluar la configuración de tu entorno en la nube, detectando fácilmente las debilidades.

Además, los agentes ligeros y multiplataforma de Wazuh se utilizan habitualmente para monitorizar entornos en la nube a nivel de instancia.

**Seguridad de contenedores**

Wazuh proporciona visibilidad de seguridad en tus hosts y contenedores Docker, monitorizando su comportamiento y detectando amenazas, vulnerabilidades y anomalías. El agente de Wazuh cuenta con integración nativa con el motor de Docker, lo que permite a los usuarios monitorizar imágenes, volúmenes, configuraciones de red y contenedores en ejecución.

Wazuh recopila y analiza continuamente información detallada en tiempo de ejecución. Por ejemplo, genera alertas para contenedores que se ejecutan en modo privilegiado, aplicaciones vulnerables, un shell ejecutándose dentro de un contenedor, cambios en volúmenes o imágenes persistentes, y otras posibles amenazas.

## WUI

La WUI de Wazuh ofrece una potente interfaz de usuario para la visualización y el análisis de datos. Esta interfaz también puede utilizarse para gestionar la configuración de Wazuh y monitorizar su estado.

**Resumen de módulos**

![Modules overview](https://github.com/wazuh/wazuh-dashboard-plugins/raw/main/screenshots/app.png)

**Eventos de seguridad**

![Overview](https://github.com/wazuh/wazuh-dashboard-plugins/blob/main/screenshots/app2.png)

**Monitorización de integridad**

![Overview](https://github.com/wazuh/wazuh-dashboard-plugins/blob/main/screenshots/app3.png)

**Detección de vulnerabilidades**

![Overview](https://github.com/wazuh/wazuh-dashboard-plugins/blob/main/screenshots/app4.png)

**Cumplimiento normativo**

![Overview](https://github.com/wazuh/wazuh-dashboard-plugins/blob/main/screenshots/app5.png)

**Resumen de agentes**

![Overview](https://github.com/wazuh/wazuh-dashboard-plugins/blob/main/screenshots/app6.png)

**Resumen del agente**

![Overview](https://github.com/wazuh/wazuh-dashboard-plugins/blob/main/screenshots/app7.png)

## Orquestación

Aquí puedes encontrar todas las herramientas de automatización mantenidas por el equipo de Wazuh.

* [Wazuh AWS CloudFormation](https://github.com/wazuh/wazuh-cloudformation)

* [Contenedores Docker](https://github.com/wazuh/wazuh-docker)

* [Wazuh Ansible](https://github.com/wazuh/wazuh-ansible)

* [Wazuh Chef](https://github.com/wazuh/wazuh-chef)

* [Wazuh Puppet](https://github.com/wazuh/wazuh-puppet)

* [Wazuh Kubernetes](https://github.com/wazuh/wazuh-kubernetes)

* [Wazuh Bosh](https://github.com/wazuh/wazuh-bosh)

* [Wazuh Salt](https://github.com/wazuh/wazuh-salt)

## Ramas (Branches)

* La rama `main` contiene el código más reciente; ten en cuenta la posibilidad de errores en esta rama.

## Software y bibliotecas utilizadas

| Software                                                                | Versión | Autor                          | Licencia                                       |
| ----------------------------------------------------------------------- | ------- | ----------------------------- | --------------------------------------------- |
| [bpftool](https://github.com/libbpf/bpftool)                            | 7.7.0   | libbpf                        | GNU Public License version 2                  |
| [bzip2](https://github.com/libarchive/bzip2)                            | 1.0.8   | Julian Seward                 | BSD License                                   |
| [cJSON](https://github.com/DaveGamble/cJSON)                            | 1.7.18  | Dave Gamble                   | MIT License                                   |
| [cpp-httplib](https://github.com/yhirose/cpp-httplib)                   | 0.25.0  | yhirose                       | MIT License                                   |
| [cPython](https://github.com/python/cpython)                            | 3.12.13 | Guido van Rossum              | Python Software Foundation License version 2  |
| [cURL](https://github.com/curl/curl)                                    | 8.20.0  | Daniel Stenberg               | MIT License                                   |
| [dbus](https://gitlab.freedesktop.org/dbus/dbus)                        | 1.14.10 | freedesktop.org               | GNU Public License version 2                  |
| [Flatbuffers](https://github.com/google/flatbuffers/)                   | 23.5.26 | Google Inc.                   | Apache 2.0 License                            |
| [Google Benchmark](https://github.com/google/benchmark)                 | 1.6.1   | Google Inc.                   | Apache 2.0 License                            |  |
| [GoogleTest](https://github.com/google/googletest)                      | 1.11.0  | Google Inc.                   | 3-Clause "New" BSD License                    |
| [jemalloc](https://github.com/jemalloc/jemalloc)                        | 5.2.1   | Jason Evans                   | 2-Clause "Simplified" BSD License             |
| [libarchive](https://github.com/libarchive/libarchive)                  | 3.8.7   | Tim Kientzle                  | 3-Clause "New" BSD License                    |
| [libbpf](https://github.com/libbpf/libbpf)                              | 1.7.0   | libbpf                        | GNU Lesser General Public License version 2.1 |
| [libdb](https://github.com/yasuhirokimura/db18)                         | 18.1.40 | Oracle Corporation            | Affero GPL v3                                 |
| [libffi](https://github.com/libffi/libffi)                              | 3.2.1   | Anthony Green                 | MIT License                                   |
| [libpcre2](https://github.com/PCRE2Project/pcre2)                       | 10.42.0 | Philip Hazel                  | BSD License                                   |
| [libplist](https://github.com/libimobiledevice/libplist)                | 2.2.0   | Aaron Burghardt et al.        | GNU Lesser General Public License version 2.1 |
| [libYAML](https://github.com/yaml/libyaml)                              | 0.1.7   | Kirill Simonov                | MIT License                                   |
| [liblzma](https://github.com/tukaani-project/xz)                        | 5.8.3   | Lasse Collin, Jia Tan et al.  | GNU Public License version 3                  |
| [Linux Audit userspace](https://github.com/linux-audit/audit-userspace) | 2.8.4   | Rik Faith                     | GNU Lesser General Public License             |
| [Lua](https://github.com/lua/lua)                                       | 5.4.8   | PUC-Rio                       | MIT License                                   |
| [nlohmann](https://github.com/nlohmann/json)                            | 3.11.2  | Niels Lohmann                 | MIT License                                   |
| [OpenSSL](https://github.com/openssl/openssl)                           | 3.6.2   | OpenSSL Software Foundation   | Apache 2.0 License                            |
| [popt](https://github.com/rpm-software-management/popt)                 | 1.16    | Jeff Johnson & Erik Troan     | MIT License                                   |
| [procps](https://gitlab.com/procps-ng/procps)                           | 2.8.3   | Brian Edmonds et al.          | GNU Lesser General Public License             |
| [RocksDB](https://github.com/facebook/rocksdb/)                         | 8.3.2   | Facebook Inc.                 | Apache 2.0 License                            |
| [rpm](https://github.com/rpm-software-management/rpm)                   | 4.20.1  | Marc Ewing & Erik Troan       | GNU Public License version 2                  |
| [simdjson](https://github.com/simdjson/simdjson)                        | 3.13.0  | Daniel Lemire                 | Apache License 2.0                            |
| [sqlite](https://github.com/sqlite/sqlite)                              | 3.53.1  | D. Richard Hipp               | Public Domain (no restrictions)               |
| [zlib](https://github.com/madler/zlib)                                  | 1.3.1   | Jean-loup Gailly & Mark Adler | zlib/libpng License                           |

* [Paquetes PyPi](framework/requirements.txt)

## Documentación

* [Documentación completa](http://documentation.wazuh.com)
* [Guía de instalación de Wazuh](https://documentation.wazuh.com/current/installation-guide/index.html)

## Participa

Forma parte de la [comunidad de Wazuh](https://wazuh.com/community/) para aprender de otros usuarios, participar en debates, hablar con nuestros desarrolladores y contribuir al proyecto.

Si deseas contribuir a nuestro proyecto, no dudes en enviar pull requests, reportar issues o enviar commits; revisaremos todas tus consultas.

También puedes unirte a nuestro [canal de comunidad en Slack](https://wazuh.com/community/join-us-on-slack/) y a la [lista de correo](https://groups.google.com/d/forum/wazuh) enviando un correo electrónico a [wazuh+subscribe@googlegroups.com](mailto:wazuh+subscribe@googlegroups.com), para hacer preguntas y participar en debates.

Mantente al día sobre noticias, lanzamientos, artículos técnicos y más.

* [Sitio web de Wazuh](http://wazuh.com)
* [Linkedin](https://www.linkedin.com/company/wazuh)
* [YouTube](https://www.youtube.com/c/wazuhsecurity)
* [Twitter](https://twitter.com/wazuh)
* [Blog de Wazuh](https://wazuh.com/blog/)
* [Canal de anuncios en Slack](https://wazuh.com/community/join-us-on-slack/)

## Autores

Wazuh Copyright (C) 2015-2023 Wazuh Inc. (Licencia GPLv2)

Basado en el proyecto OSSEC iniciado por Daniel Cid.
