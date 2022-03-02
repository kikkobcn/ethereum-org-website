---
titolo: Introdución a ether
descripción: Introducción de un desarrollador a la criptomoneda ether.
lang: es
sidebar: true
---

## Prerequisitos {#prerequisitos}

Para entender mejor esta pagina, te recomendamos leer primero [Introduction to Ethereum](/developers/docs/intro-to-ethereum/).

## Que es una criptomoneda? {#Que-es-una-criptomoneda}

Una criptomoneda es un medio de intercambio asegurado por un ledger basado en blockchain.

Un medio de intercambio es cualquier cosa ampliamente aceptada como pago por bienes y servicios, y un libro de contabilidad es un almacén de datos que mantiene un registro de las transacciones. La tecnología Blockchain permite a los usuarios realizar transacciones en el libro de contabilidad sin depender de un tercero de confianza para mantener el libro de contabilidad.

La primera criptomoneda fue Bitcoin, creada por Satoshi Nakamoto. Desde el lanzamiento de Bitcoin en 2009, la gente ha creado miles de criptodivisas en muchas cadenas de bloques diferentes.

## ¿Qué es el éter? {#what-is-ether}

**Ether (ETH)** es la criptomoneda utilizada para muchas cosas en la red Ethereum. Fundamentalmente, es la única forma de pago aceptable para las tarifas de las transacciones, y después de [La Fusión](/upgrades/merge) también se requiere para validar y proponer bloques en Mainnet. El éter también se utiliza como forma principal de garantía en los mercados de préstamos [DeFi](/defi), como unidad de cuenta en los mercados NFT, como pago obtenido por la realización de servicios o la venta de bienes del mundo real, y mucho más.

Ethereum permite a los desarrolladores crear [**aplicaciones descentralizadas (dapps)**](/desarrolladores/docs/dapps), que comparten un conjunto de potencia de cálculo. Esta reserva compartida es finita, por lo que Ethereum necesita un mecanismo para determinar quién puede utilizarla. De lo contrario, una dapp podría consumir accidentalmente o de forma maliciosa todos los recursos de la red, lo que bloquearía el acceso de los demás.

La criptomoneda ether soporta un mecanismo de precios para la potencia de cálculo de Ethereum. Cuando los usuarios quieren hacer una transacción, deben pagar ether para que su transacción sea reconocida en la blockchain. Estos costes de uso se conocen como [tasas de gas](/developers/docs/gas/), y la tasa de gas depende de la cantidad de potencia de cálculo necesaria para ejecutar la transacción y de la demanda de potencia de cálculo en toda la red en ese momento.

Por lo tanto, incluso si una dapp maliciosa presentara un bucle infinito, la transacción acabaría quedándose sin éter y terminaría, permitiendo que la red volviera a la normalidad.

Es [común](https://www.reuters.com/article/us-crypto-currencies-lending-insight-idUSKBN25M0GP#:~:text=price%20of%20ethereum) [to](https://abcnews.go.com/Business/bitcoin-slumps-week-low-amid-renewed-worries-chinese/story?id=78399845#:~:text=cryptocurrencies%20including%20ethereum) [conflate](https://www.cnn.com/2021/03/14/tech/nft-art-buying/index.html#:~:text=price%20of%20ethereum) Ethereum y éter - cuando la gente hace referencia al "precio de Ethereum", están describiendo el precio del éter.

## Acuñación del éter {#minting-ether}

La acuñación es el proceso en el que se crea nuevo éter en el libro mayor de Ethereum. El protocolo subyacente de Ethereum crea el nuevo éter, y no es posible que un usuario cree éter.

El éter se acuña cuando un minero crea un bloque en la cadena de bloques de Ethereum. Como incentivo para los mineros, el protocolo concede una recompensa en cada bloque, incrementando el saldo de una dirección establecida por el minero del bloque. La recompensa por bloque ha cambiado con el tiempo, y hoy en día es de 2 ETH por bloque.

## Quemar éter {#burning-ether}

Además de crear éter a través de las recompensas de los bloques, el éter puede destruirse mediante un proceso llamado "quema". Cuando el éter se quema, se retira de la circulación de forma permanente.

La quema de éter se produce en cada transacción en Ethereum. Cuando los usuarios pagan por sus transacciones, el protocolo destruye el éter base. Dependiendo de la demanda de la red, [algunos bloques](https://etherscan.io/block/12965263) queman más éter del que acuñan.


## Denominaciones de ether {#denominaciones}

Dado que muchas transacciones en Ethereum son pequeñas, el ether tiene varias denominaciones que pueden ser referenciadas para cantidades más pequeñas. De estas denominaciones, Wei y gwei son particularmente importantes.

Wei es la cantidad más pequeña posible de ether, y como resultado, muchas implementaciones técnicas, como el [Ethereum Yellowpaper](https://ethereum.github.io/yellowpaper/paper.pdf), basarán todos los cálculos en Wei.

Gwei, abreviatura de giga-wei, se utiliza a menudo para describir los costes de gas en Ethereum.


| Denominacion | Valor en ether   | Uso Comun                 |
| ------------ | ---------------- | ------------------------- |
| Wei          | 10<sup>-18</sup> | Technical implementations |
| Gwei         | 10<sup>-9</sup>  | Human-readable gas fees   |

## Transferencia de éter {#transferring-ether}

Cada transacción en Ethereum contiene un campo `valor`, que especifica la cantidad de ether a transferir, denominada en wei, para enviar desde la dirección del remitente a la del destinatario.

Cuando la dirección del destinatario es un [contrato inteligente](/developers/docs/smart-contracts/), este éter transferido puede utilizarse para pagar el gas cuando el contrato inteligente ejecuta su código.

[Más sobre las transacciones](/developers/docs/transactions/)

## Consulta del éter {#Consulta del éter}

Los usuarios pueden consultar el saldo de éter de cualquier [cuenta](/developers/docs/accounts/) inspeccionando el campo `balance` de la cuenta, que muestra las tenencias de éter denominadas en wei.

[Etherscan](https://etherscan.io) es una herramienta popular para inspeccionar los balances de las direcciones a través de una aplicación basada en la web. Por ejemplo, [esta página de Etherscan](https://etherscan.io/address/0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae) muestra el balance de la Fundación Ethereum.

## Lectura adicional {#further-reading}

- [Definición de Ether y Ethereum](https://www.cmegroup.com/education/courses/introduction-to-ether/defining-ether-and-ethereum.html) - _CME Group_
- [Ethereum Whitepaper](/whitepaper/): La propuesta original de Ethereum. Este documento incluye una descripción del éter y las motivaciones para su creación.

¿Conoces algún recurso de la comunidad que te haya ayudado? Edita esta página y añádelo.
