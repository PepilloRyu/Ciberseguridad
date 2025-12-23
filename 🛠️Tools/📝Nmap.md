Se llama Network Mapper
Es una herramienta de líneas de comandos de código abierto que se utiliza para escanear:
- Direcciones IP
- Puertos de una red
- Dispositivos conectados a una red
- Servicios y posibles vulnerabilidades

Permite encontrar que dispositivos están en la red que se desea escanear detectar vulnerabilidades.

### Descubrimiento de hosts

```bash
-sn # Detecta hosts activos sin escanear puertos
```

```bash
-Pn # Asume host activo (omite ping)
```

```bash
-n # No resuelve DNS
```

```bash
-R # Fuerza resolución DNS
```

```bash
--traceroute # Muestra ruta al host
```

### Puertos

```bash
-p # Define puertos específicos
```

```bash
-p- # Escanea todos los puertos
```

```bash
--top-ports # Escanea puertos más comunes
```

```bash
--open # Muestra solo puertos abiertos
```

### Tipos de escaneo
```bash
-sS # TCP SYN (sigiloso)
```

```bash
-sT # TCP completo
```

```bash
-sU # UDP
```

```bash
-sA # ACK (firewalls)
```

```bash
-sN # NULL
```

```bash
-sF # FIN
```

```bash
-sX # Xmas
```

### Detección
```bash
-sV # Versiones de servicios
```

```bash
-sC # Scripts por defecto
```

```bash
-O # Sistema operativo
```

```bash
-A # Detección agresiva
```


### Velocidad/tiempo
```bash
-T0 # Control de velocidad (Muy lento)
```

```bash
-T1 # Control de velocidad (Lento)
```

```bash
-T2 # Control de velocidad (Moderado)
```

```bash
-T3 # Control de velocidad (Normal)
```

```bash
-T4 # Control de velocidad (Rápido)
```

```bash
-T5  # Control de velocidad (Muy rápido)
```

```bash
--scan-delay # Retraso entre paquetes
```

```bash
--max-rate # Máx paquetes/seg
```

```bash
--min-rate # Mín paquetes/seg
```

```bash
--max-retries # Reintentos
```

```bash
--host-timeout # Tiempo máximo por host
```

### NSE (SCRIPTS)
```bash
--script # Ejecuta scripts NSE
```

```bash
--script-vuln # Busca vulnerabilidades
```


### Salida
```bash
-oN # Texto normal
```

```bash
-oX # XML
```

```bash
-oG # Grepable
```

```bash
-oA # Todas las salidas
```

### Verbosidad
```bash
-v # Verbose
```

```bash
--vv # Verbose avanzado
```

```bash
-d # Debug
```

```bash
-dd # Debug avanzado
```

```bash
--reason # Explica estados
```

### Red
```bash
--dns-servers # Usa DNS personalizados
```

```bash
-6 # IPv6
```

```bash
--iflist # Interfaces
```

### Evasión 
```bash
--mtu # Fragmenta paquetes
```

```bash
--data-length # Relleno de paquetes
```

```bash
--spoof-mac # Falsifica MAC
```

```bash
--source-port # Puerto de origen falso
```

```bash
--randomize-hosts # Orden aleatorio
```

### Control
```bash
--exclude # Excluye hosts
```

```bash
--exclude-file # Excluye desde archivo
```

```bash
--resume # Reanuda escaneo
```

### Sistema
```bash
--privileged
```

### Comandos listos para usar
#### CTF rápido
```bash
nmap -p- -sV -sC -Pn -n -T4 --open <IP>
```

#### Pentesting más sigiloso
```bash
nmap -p- -sV -sC -Pn -n -T2 --scan-delay 500ms <IP>
```
