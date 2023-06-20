# Miso-grupo18-modernizacion-software

En el siguiente proyecto se plantea la siguiente aplicacion base para modernizar: [Link AQUI](https://github.com/GoogleCloudPlatform/monolith-to-microservices-example)
 
Pasando de una aplicacion de monolito a una aplicacion de micro servicios.

## Funcionamieto de la aplicacion

La aplicacion cuenta con los siguientes endpoints:

- Home  muestra todos los productos GET = /

- Obtener producto GET = /product/{id}

- Guardar las configuraciones del carro de compras POST = /cart/checkout

- Configurar características de los productos a comprar del carro de compras POST = /cart

- Mostrar el carro de compras como va hasta el momento POST = /showcart

- Nos ayuda a quitar productos del carro de comprasPOST = /cart/empty

La aplicación nos ayuda a crear un carro de compras con diferentes productos que vayamos escogiendo  

## Ejecutar la aplicacion con docker

- ingresar a la carpeta monolith
- ejecutar
```shell
docker build --tag java-docker . 
```
y despues

```shell
 docker run -d -p 8089:8080 java-docker
```