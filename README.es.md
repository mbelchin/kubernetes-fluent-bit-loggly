# Kubernetes usando FluentBit para enviar logs a Loggly
> Configura Fluent Bit para ejecutarse dentro de un cluster de Kubernetes y enviar logs de tus pods a Loggly

![GitHub](https://img.shields.io/github/license/mbelchin/kubernetes-fluent-bit-loggly.svg)
![GitHub release](https://img.shields.io/github/release/mbelchin/kubernetes-fluent-bit-loggly.svg)


[![Twitter](https://img.shields.io/twitter/url/https/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fmbelchin%2Fkubernetes-fluent-bit-loggly&hashtags=kubernetes,fluentbit,loggly,daemontset,serviceaccount,configmap,secrets)

*Lee esta información en otros idiomas: [English](README.md), [Español](README.es.md).*

Configura Fluent Bit para ejecutarse dentro de un cluster de Kubernetes y enviar logs de tus pods a Loggly

![](kubernetes-fluentbit-loggly.jpg)

## Instalación

Dentro de tu cluster Kubernetes

```
$ kubectl create -f fluent-bit-service-account.yaml

$ kubectl create -f fluent-bit-secrets-loggly.yaml

$ kubectl create -f fluent-bit-configmap-loggly.yaml

$ kubectl create -f fluent-bit-ds-loggly.yaml
```

## Ejemplo de uso

_Para obtener una información más detallada acerca de este paquete, por favor, dirígete a [https://moisesbm.wordpress.com/2018/08/25/kubernetes-with-fluent-bit-to-send-logs-to-loggly/](https://moisesbm.wordpress.com/2018/08/25/kubernetes-with-fluent-bit-to-send-logs-to-loggly/)._

## Autor

[Moisés Belchín](https://moisesbm.wordpress.com)  
[@moises_b_m](https://twitter.com/moises_b_m)  
[https://github.com/mbelchin/](https://github.com/mbelchin/)  

Distribuido bajo lincencia MIT. Echa un vistazo a ``LICENSE`` para más información.

## Documentación

Para obtener una información más detallada acerca de este paquete, por favor, dirígete a :
[https://moisesbm.wordpress.com/2018/08/25/kubernetes-with-fluent-bit-to-send-logs-to-loggly/](https://moisesbm.wordpress.com/2018/08/25/kubernetes-with-fluent-bit-to-send-logs-to-loggly/)

## Discusión

Este proyecto fue creado para encontrar una forma simple de configurar FluentBit dentro de un cluster de Kubernetes y enviar los logs de tus pods a una cuenta Loggly.

Si consideras que algunas cosas podrían mejorarse o si conoces alguna otra herramienta más sencilla, por favor, abre un hilo de debate para que todos nos podamos beneficiar de todas las mejoras que surjan.

## Contribuir

1. Haz un fork (<https://github.com/mbelchin/kubernetes-fluent-bit-loggly/fork>)
2. Crea una nueva rama (`git checkout -b feature/fooBar`)
3. Haz un commit de tus cambios (`git commit -am '<type>(scope): add some fooBar'`)
4. Haz push de tu rama (`git push origin feature/fooBar`)
5. Crea un nuevo Pull Request
