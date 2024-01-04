🔒 **point-c**: Seamless Integration of [Caddy](https://caddyserver.com/) with [WireGuard](https://www.wireguard.com/) in pure Go

Welcome to `point-c`! This project is designed to provide a robust and fully integrated solution for running Caddy web server over the secure WireGuard VPN, all powered by the efficiency and flexibility of the Go programming language.
The goal of this project is to provide flexible and secure web traffic management.

🧩 **Modular Design**: We've taken care to break down functionality into reusable packages. This modular approach enables other applications to leverage individual components of `point-c`, making it versatile and adaptable to various use cases.

🚀 **Easy Feature Extension**: We're committed to making it easier for you to extend and enhance the functionality of `point-c`.

🌐 Explore our documentation and get started today to experience the synergy of Caddy and WireGuard with `point-c`. Secure, efficient, and ready to power your web projects!

### Suggested Use Case

The primary use case of `point-c` is to set up Caddy in a WireGuard server configuration on a VPS in the cloud, forwarding traffic to a Caddy setup in a client configuration located anywhere capable of connecting to the server. This flexible setup allows you to change the location or IP of the remote Caddy server at any time.

### Why Forward Traffic Through the Tunnel?

Forwarding traffic through the tunnel ensures that it is TLS encrypted before getting wrapped by WireGuard, and completely decrypted on the client side, which then re-encrypts it entirely. This approach ensures that if the WireGuard server is ever compromised, your traffic remains secure due to TLS encryption, with keys securely stored on the local client side.

### Compatibility and Security

Since this project utilizes official WireGuard libraries, the WireGuard traffic is compatible with any client or server. This interoperability, combined with robust TLS encryption and the efficiency of Caddy and WireGuard, makes `point-c` a powerful tool for secure and versatile web traffic management.
