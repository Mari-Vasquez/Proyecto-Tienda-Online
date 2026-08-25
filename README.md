Markdown
# Tienda Online (Flask + PostgreSQL)

Sistema de tienda online desarrollado con Python, Flask, PostgreSQL y Bootstrap para la gestión de catálogo de productos físicos, digitales y perecibles, autenticación por roles y carrito de compras.

## 🚀 Requisitos e Instalación

### 1. Clonar el repositorio
```bash
git clone [https://github.com/Mari-Vasquez/Proyecto-Tienda-Online.git](https://github.com/Mari-Vasquez/Proyecto-Tienda-Online.git)
cd Proyecto-Tienda-Online
2. Crear y activar el entorno virtual
Bash
python -m venv venv
# En Windows:
venv\Scripts\activate
# En Linux/Mac:
source venv/bin/activate
3. Instalar dependencias
Bash
pip install -r requirements.txt
4. Configurar la Base de Datos PostgreSQL
Asegúrate de tener PostgreSQL ejecutándose y ajusta las variables en config.py:

Plaintext
DATABASE_URL=postgresql://postgres:tu_contraseña@localhost:5432/tienda_online
SECRET_KEY=tu_clave_secreta
5. Inicializar la base de datos y ejecutar la app
Bash
python init_db.py
flask run
🔑 Credenciales de Prueba
Administrador:

Email: admin@tienda.com

Contraseña: admin123

Cliente:

Email: cliente@tienda.com

Contraseña: cliente123

📸 Capturas de Pantalla
Catálogo de Productos
### Catálogo de Productos
![Catálogo](static/uploads/catalogo.png)
Detalle del Producto
### Detalle del Producto
![Detalle](static/uploads/detalle.png)
Carrito de Compras
### Carrito de Compras
![Carrito](static/uploads/carrito.png)

---

**2. Verificar que `static` no esté en `.gitignore`**

Asegúrate de que en tu archivo `.gitignore` no esté incluida la palabra `static`, para que Git reconozca la carpeta `static/uploads` con las imágenes de los productos.

---

**3. Subir los cambios actualizados a GitHub**

Abre la terminal en VS Code y ejecuta los siguientes tres comandos:

```bash
git add .
git commit -m "Añadidos README.md y carpeta static con imagenes"
git push -u origin main