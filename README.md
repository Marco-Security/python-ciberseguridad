# Python Ciberseguridad

Colección de 30 retos de programación enfocados en ciberseguridad, desarrollados en Python 3 usando Jupyter Notebooks en VSCode.

## Descripción

Cada reto incluye un enunciado, pistas progresivas y una celda de código para implementar la solución. Los ejercicios van de fundamentos a detección, cubriendo las áreas más relevantes para un perfil SOC Analyst / Pentester.

## Módulos

| Módulo | Tema | Retos |
|--------|------|-------|
| 1 | Criptografía | Hashing, cifrado César, AES-256, fuerza bruta MD5, generador de passwords |
| 2 | Redes y Escaneo | Port scanner, banner grabbing, DNS inverso, geolocalización IP, sniffer |
| 3 | Análisis Web | Headers HTTP, SQLi, XSS, directory brute-force, extractor de formularios |
| 4 | Forense Digital | Hash de archivos, metadatos EXIF, análisis de logs, archivos sensibles, strings en binarios |
| 5 | Exploits y Post-Explotación | Encoder Base64, fuzzer HTTP, bind shell, detector LFI, keylogger |
| 6 | Blue Team / Detección | Detector port scan, parser Wazuh, análisis PCAP, correlación de eventos, reporte de incidente |

## Stack

- Python 3.13
- Jupyter Notebook (VSCode)
- Librerías: `cryptography`, `requests`, `scapy`, `Pillow`, `pynput`, `beautifulsoup4`

## Setup

```bash
# Clonar el repositorio
git clone https://github.com/Marco-Security/python-ciberseguridad.git
cd python-ciberseguridad

# Crear entorno virtual
python -m venv venv
.\venv\Scripts\Activate.ps1  # Windows
source venv/bin/activate      # Linux/Mac

# Instalar dependencias
pip install cryptography requests scapy Pillow pynput beautifulsoup4 ipykernel

# Registrar kernel en Jupyter
python -m ipykernel install --user --name=venv_ciberseg --display-name "Python (ciberseg)"
```

Abrir `ejercicios_ciberseguridad.ipynb` en VSCode y seleccionar el kernel **Python (ciberseg)**.

## Aviso Legal

Los ejercicios de este repositorio son exclusivamente para fines educativos. Las técnicas de escaneo, fuzzing y explotación deben practicarse únicamente en entornos propios o con autorización explícita. El uso indebido de estas técnicas puede tener consecuencias legales.
