# Kubernetes using FluentBit to send logs to Loggly
> Configure Fluent Bit to run inside Kubernetes cluster to send logs to Loggly

![GitHub](https://img.shields.io/github/license/mbelchin/kubernetes-fluent-bit-loggly.svg)
![GitHub release](https://img.shields.io/github/release/mbelchin/kubernetes-fluent-bit-loggly.svg)


[![Twitter](https://img.shields.io/twitter/url/https/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fmbelchin%2Fkubernetes-fluent-bit-loggly&hashtags=git,hooks,developers,commit,format)

*Read this in other languages: [English](README.md), [Español](README.es.md).*

Configure Fluent Bit to run inside a Kubernetes cluster to send logs to Loggly

![](kubernetes-fluentbit-loggly.jpg)

## Installation

In your kubernetes cluster

```
$ kubectl create -f fluent-bit-service-account.yaml

$ kubectl create -f fluent-bit-secrets-loggly.yaml

$ kubectl create -f fluent-bit-configmap-loggly.yaml

$ kubectl create -f fluent-bit-ds-loggly.yaml
```

## Usage example

_For more examples and usage, please refer to [https://moisesbm.wordpress.com/2018/08/25/kubernetes-with-fluent-bit-to-send-logs-to-loggly/](https://moisesbm.wordpress.com/2018/08/25/kubernetes-with-fluent-bit-to-send-logs-to-loggly/)._

## Author

[Moisés Belchín](https://moisesbm.wordpress.com)  
[@moises_b_m](https://twitter.com/moises_b_m)  
[https://github.com/mbelchin/](https://github.com/mbelchin/)  

Distributed under the MIT license. See ``LICENSE`` for more information.

## Documentation

For a detailed explanation, please refer to:
[https://moisesbm.wordpress.com/2018/08/25/kubernetes-with-fluent-bit-to-send-logs-to-loggly/](https://moisesbm.wordpress.com/2018/08/25/kubernetes-with-fluent-bit-to-send-logs-to-loggly/)

## Discussion

This project was created to find a simple way to configure FluentBit inside a Kubernetes cluster to send logs to a Loggly account.

If you consider some things could be improved or you know another simpler, easier configurable tools, please open a discussion thread so all of us could benefit from those improvements.

## Contributing

1. Fork it (<https://github.com/mbelchin/kubernetes-fluent-bit-loggly/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am '<type>(scope): add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request
