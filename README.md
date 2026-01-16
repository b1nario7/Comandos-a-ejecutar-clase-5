# Comandos-a-ejecutar-clase-5

Primero descargar Python e instalar:
https://www.python.org/downloads/

Luego en PowerShell como administradores:
`winget install --id Git.Git -e --source winget`

`git clone https://github.com/volatilityfoundation/volatility3.git`

`cd volatility3/`

`python -m venv venv`

`Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass`
Colocan Y

`.\venv\Scripts\Activate.ps1`

`pip install -e .`

Copiar memory.raw dentro de la carpeta volatility3 o usar la ruta completa al archivo


Para las preguntas:

Sistema operativo
`python vol.py -f memory.raw windows.info`

Procesos activos
`python vol.py -f memory.raw windows.pslist`
`python vol.py -f memory.raw windows.psscan`

Línea de comando
`python vol.py -f memory.raw windows.cmdline`
