# Spec: Python Ping Server

## Descripción

Implementar un servidor HTTP en Python que exponga un endpoint `/ping` que retorne `pong`.

## Requisitos

### Endpoint

| Método | URL    | Respuesta |
|--------|--------|-----------|
| GET    | /ping  | `pong`    |

### Detalles técnicos

- El servidor debe estar escrito en **Python**.
- Al realizar una petición `GET /ping`, el servidor debe responder con el texto `pong` y código de estado HTTP `200`.
- El servidor debe escuchar en el puerto `8000` por defecto.

## Ejemplo de uso

Iniciar el servidor:

```bash
python server.py
```

Verificar el endpoint:

```bash
curl http://localhost:8000/ping
# Respuesta esperada: pong
```

## Criterios de aceptación

- [ ] El servidor arranca sin errores.
- [ ] `GET /ping` responde con el cuerpo `pong` y estado `200`.
- [ ] El código no requiere dependencias externas (sólo la librería estándar de Python).
