# 🎉 Bienvenido a **PeruSCP** 🚀

[![Version](https://img.shields.io/badge/version-0.0.1-blue)](https://github.com/perusrc) [![Python](https://img.shields.io/badge/python-3.7%2B-green)](https://python.org) [![Status](https://img.shields.io/badge/status-active-success)](https://eldni.com)

**PeruSCP** es una librería de Python diseñada para simplificar el acceso a datos del Registro Nacional de Identificación en Perú. A través de esta herramienta, puedes obtener información personal asociada a un DNI (Documento Nacional de Identidad) utilizando técnicas de web scraping en sitios autorizados. 🧾

## 📦 **Módulo `eldni`**

Este módulo te permite enviar un DNI válido y obtener los siguientes datos:

- 👤 **Nombre**
- 🧔 **Apellido paterno**
- 👩 **Apellido materno**
- 🆔 **Nombre completo**

Toda esta información es extraída dinámicamente desde [eldni.com](https://eldni.com/), lo que te asegura datos actualizados en todo momento.

## 🚀 **Instalación**

Puedes instalar `PeruSCP` fácilmente usando `pip`:

```bash
pip install peruscp
```

## ✨ **Uso del módulo `elDNI`**

A continuación te mostramos cómo puedes usar el módulo `elDNI` para obtener datos a partir de un DNI:

```python
from peruscp import elDNI

# Ingresa el DNI que quieres consultar
datos = elDNI.consultaDni(27427864)

# Imprime la información obtenida
print(datos)
```

### 📝 **Ejemplo de salida:**

```json
{
   "Status":true,
   "datos":{
      "Nombre":"JOSE PEDRO",
      "ApellidoP":"CASTILLO",
      "ApellidoM":"TERRONES",
      "NombreCompleto":"JOSE PEDRO CASTILLO TERRONES",
      "Fuente":"https://eldni.com/"
   }
}
```

## ⚖️ **Licencia**

Este proyecto está bajo la licencia [MIT](LICENSE).

---

📫 **Contacto**: Si tienes alguna pregunta o inquietud, no dudes en contactarnos a través de [bryanpinzon469@gmail.com](bryanpinzon469@gmail.com).

¡Gracias por usar **PeruSCP**! ✨👩‍💻👨‍💻
