### **Instalación/Actualización de PHP 8.2, Composer 2.x y Node.js 18.x con npm**
- [ ] PHP 8.2.12 instalado con extensiones necesarias (`bcmath`, `mbstring`, `xml`, `curl`, `mysql`, `zip`, `opcache`).
- [x] Composer version 2.8.3
- [ ] Node.js v22.11.0
- [ ] npm 10.9.0

#### **1. PHP 8.2 con extensiones necesarias**

##### **a. Comando para instalar PHP 8.2 y habilitar extensiones**
Comandos:

```bash
sudo add-apt-repository ppa:ondrej/php -y
sudo apt update
sudo apt install -y php8.2 php8.2-cli php8.2-mbstring php8.2-xml php8.2-curl php8.2-mysql php8.2-bcmath php8.2-zip php8.2-opcache
```

---

##### **b. Detalles:**

1. **`php8.2`**  
   Instala PHP 8.2, el motor necesario para ejecutar Laravel 11.

2. **`php8.2-cli`**  
   Proporciona herramientas de línea de comandos para ejecutar comandos como `artisan` o scripts PHP directamente.

3. **Extensiones habilitadas:**
   - **`php8.2-bcmath`**:  
     Habilita funciones matemáticas de precisión arbitraria necesarias para ciertos cálculos en Laravel.
   - **`php8.2-mbstring`**:  
     Permite trabajar con cadenas de caracteres multibyte (como UTF-8), esencial para manejar textos.
   - **`php8.2-xml`**:  
     Proporciona soporte para leer y escribir documentos XML, necesario para integraciones o análisis de datos.
   - **`php8.2-curl`**:  
     Permite realizar solicitudes HTTP, esencial para trabajar con APIs externas.
   - **`php8.2-mysql`**:  
     Habilita la conexión de PHP con bases de datos MySQL o MariaDB.
   - **`php8.2-zip`**:  
     Agrega soporte para comprimir y descomprimir archivos ZIP, necesario para algunas operaciones en Laravel.
   - **`php8.2-opcache`**:  
     Optimiza el rendimiento almacenando en caché los scripts PHP compilados.

---

#### **2. Composer 2.x**

##### **a. Comando para instalar Composer**
Comandos:
```bash
sudo apt install -y composer
```

##### **b. Detalle:**
Composer es un gestor de dependencias para PHP que permite instalar y actualizar librerías necesarias para Laravel y otros proyectos PHP.

---

#### **3. Node.js 18.x con npm**

##### **a. Comando para instalar Node.js 18.x**
Comandos:
```bash
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs
```

##### **b. Detalles:**
1. **`curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -`**  
   Descarga y configura el repositorio oficial de Node.js 18.x.

2. **`sudo apt install -y nodejs`**  
   Instala Node.js y npm (el gestor de paquetes de Node.js) en el servidor.
