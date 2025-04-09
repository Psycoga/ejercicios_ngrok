## Instalación y configuración de ngrok
### Instalación

```bash
sudo apt install ngrok
```
### Configuración

```bash
ngrok config add-authtoken <token>
```
### Ejemplo de uso
- Lo que vamos a hacer para probar que funciona es levantar un servidor web en el puerto 8000 y exponerlo a internet con python, acto seguido ejecutamos ngrok, con el siguiente comando:

```bash
ngrok http http://localhost:8000
```

![alt text](/ANEXOS/image.png)

### Crear dominio con ngrok
![alt text](/ANEXOS/image_1.png)


