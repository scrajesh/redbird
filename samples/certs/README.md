# Self signed SSL certs

Created with:

```bash
$ openssl genrsa -out dev-key.pem 1024
$ openssl req -new -key dev-key.pem -out dev-csr.pem
$ openssl x509 -req -in dev-csr.pem -signkey dev-key.pem -out dev-cert.pem
```
