# ShellOverMqtt

This project aims to provide a secure and lightweight solution for remote shell forwarding using a public MQTT server. The goal is to enable secure transmission of data over the public network, even when using the TCP protocol on a public MQTT broker.

This project is based on Python and the **[paho.mqtt.python](https://github.com/eclipse/paho.mqtt.python)**.

## Features

- Randomized topic generation using TOTP (Time-based One-Time Password) to increase the difficulty of targeted monitoring on large public brokers and prevent topic abuse attacks.
- End-to-end encryption of the payload to ensure confidentiality and integrity of the transmitted data.
- Message authentication using MIC and sequence number to prevent replay attacks and ensure the authenticity of the messages.
- Support for TLS connection to a trusted CA when using MQTT to mitigate man-in-the-middle attacks. (Implemented via paho-mqtt)

## Roadmap

The project will be developed in stages, starting from a simple implementation and gradually progressing to a more secure and feature-rich solution:

1. **Basic Implementation**: Develop a single-server, single-state implementation with basic application-layer data encapsulation and rules.
2. **Payload Encryption**: Implement payload encryption to provide end-to-end security, even when the transmission layer is not secure.
3. **Enhanced Security Measures**: Introduce additional security mechanisms to prevent common attacks such as replay attacks and man-in-the-middle attacks.

## Contributing

Contributions to the project are welcome! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request.



---

Please note that the project is currently in the very early stages of development, and the initial version is being actively worked on by the project maintainer, a student. As a result, the maintenance and updates may be relatively very slow. Your patience and understanding are greatly appreciated.