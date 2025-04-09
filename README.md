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

- Esto sirve para que solo tengas un dominio, en vez de un dominio diferente cada vez que inicias ngrok.

![alt text](/ANEXOS/image_1.png)

- Una vez que hayas creado el dominio, podemos entrar por el con:
```bash
ngrok http 8000 --url https://decent-awake-lobster.ngrok-free.app
```

![alt text](/ANEXOS/image_2.png)


### Hacer ngrok mas seguro
- Si no quieres que todo el mundo pueda entrar en tu página, puede utilizar el siguiente comando:
```bash
ngrok http http://localhost:8000 --oauth google --oauth-allow-email email@example.com
```

