
## Para sacar los certificados chain de un fichero .pfx o .p12 y con los parametros de openssl no funciona podemos realizar los siguientes pasos

### Para sacar el certificado en formato p7b utilizar windows y exportat en formato pkcs7

openssl pkcs7 -inform der -in cert.p7b  -out cert.pem
openssl pkcs7 -print_certs -in cert.pem  -out cert.pem2
