# Comandos para proyectos de Nest

## Creacion de un proyecto

1. Comando para crear un proyecto en Nest JS
```bash
$   nest new <nombre>
```

2. Agregar Prisma ORM para coneccion a bases de datos

```bash
$   npm install prisma --save-dev
# y luego
$   npx prisma init
```

3. Instalaciones para validacion de variables de entorno
```bash
$   npm install joi dotenv
```

4. Generar cliente de Prisma
```bash
$   npx prisma generate
```

5. Migración de la base de datos (solo en BD relacionales)
```bash
$   npx prisma migrate dev --name <nombre-de-la-migracion>
```

6. Creacion de documento (solo en MongoDb)
```bash
$   npx prisma db push
```

7. Instalacion de dependecias de microservicios
```bash
$   npm i @nestjs/microservices nats
```

8. Instalacion de Validators y Transformers
```bash
$   npm i class-validator class-transformer
```


## Creacion de modulos, recursos y controladores

1. Creacion de un recurso entero (sin archivos spec)

```bash
$   nest g res <nombre> --no-spec
```

## Crear imagen y subir a Docker Hub

1. Creacion de la imagen independiente
```bash
$   docker build -t <usuario>/<nombre-imagen> .
```

2. Subir a repositorio de Docker Hub
```bash
$   docker push <usuario>/<nombre-imagen>:tagname
```