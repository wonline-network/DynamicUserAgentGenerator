# DynamicUserAgentGenerator
[![Latest Stable Version](https://poser.pugx.org/wonline-network/dynamic-user-agent-generator/v)](https://packagist.org/packages/wonline-network/dynamic-user-agent-generator)
[![Total Downloads](https://poser.pugx.org/wonline-network/dynamic-user-agent-generator/downloads)](https://packagist.org/packages/wonline-network/dynamic-user-agent-generator)
[![License](https://poser.pugx.org/wonline-network/dynamic-user-agent-generator/license)](https://packagist.org/packages/wonline-network/dynamic-user-agent-generator)

El `DynamicUserAgentGenerator` es una clase PHP diseñada para generar dinámicamente cadenas de agentes de usuario. Soporta una variedad de sistemas operativos incluyendo Windows, Linux, Mac, Android e iOS, con capacidades para versionado dinámico y ajustes específicos del dispositivo. Esta clase es particularmente útil para pruebas de aplicaciones web en diferentes navegadores, sistemas operativos y dispositivos simulando una amplia gama de cadenas de agentes de usuario.

## Características

- Generación dinámica de agentes de usuario.
- Soporte para sistemas operativos de escritorio y móviles.
- Técnicas de randomización para producir cadenas variadas y realistas.
- Fácil de integrar y utilizar en proyectos PHP.

## Requisitos

- PHP 7.0 o superior.

## Instalación

No se requiere una instalación específica, simplemente descargue o clone el repositorio en su proyecto y asegúrese de incluir la clase en su script PHP.

```php
require_once 'path/to/DynamicUserAgentGenerator.php';
```

## Uso

Para utilizar la clase `DynamicUserAgentGenerator`, primero debe instanciarla y luego llamar a uno de sus métodos para generar una cadena de agente de usuario. A continuación se muestra un ejemplo básico de uso:

```php
$userAgentGenerator = new DynamicUserAgentGenerator();

// Generar un agente de usuario aleatorio
echo $userAgentGenerator->generate();

// Obtener un agente de usuario para un sistema operativo específico
echo $userAgentGenerator->getOS('windows');

// Obtener un agente de usuario para un dispositivo móvil específico
echo $userAgentGenerator->getMobileOS('android');
```

## Métodos

- `generate($userAgent = NULL)`: Genera una cadena de agente de usuario aleatoria o basada en el tipo de navegador proporcionado.
- `getOS($os = NULL)`: Obtiene una cadena de agente de usuario para un sistema operativo específico.
- `getMobileOS($os = NULL)`: Obtiene una cadena de agente de usuario para un dispositivo móvil específico.

## Contribuir

Las contribuciones son bienvenidas. Si desea contribuir, por favor haga un fork del repositorio y envíe un pull request.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Vea el archivo `LICENSE` para más detalles.


## Contribuciones y soporte
#### Este proyecto ha sido creado por [Wonline](https://wonline.network).

[<img src="https://marca.wonline.io/wonline-logo.png" alt="Wonline" width="350"/>](https://wonline.network)