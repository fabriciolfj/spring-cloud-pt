# Spring vault
- Neste artigo, você aprenderá como configurar o mecanismo Vault PKI e integrá-lo ao Spring WebFlux. Com o Vault PKI, você pode gerar facilmente certificados X.509 assinados pela CA. Então, seu aplicativo pode obter um certificado por meio de uma API REST. Seu TTL é relativamente curto. É exclusivo para cada instância do aplicativo. Além disso, podemos usar Spring VaultTemplate para simplificar a integração com a API do Vault.
- Vamos falar um pouco mais sobre o Vault. Ele permite que você proteja, armazene e controle o acesso a tokens, senhas, certificados e chaves de criptografia usando UI, CLI ou API HTTP. É uma ferramenta realmente poderosa. Com o Vault, em vez de uma abordagem tradicional, você pode gerenciar sua segurança de uma maneira mais dinâmica e nativa da nuvem. Por exemplo, você pode integrar o Vault com um back-end de banco de dados e, em seguida, gerar login de usuário e senha imediatamente. Além disso, para aplicativos Spring Boot, você pode aproveitar as vantagens do projeto Spring Cloud Vault. Se você estiver interessado em obter mais informações sobre isso, leia meu artigo Testando a integração do Spring Boot com o Vault e Postgres usando Testcontainers.
- Isso não é tudo. Você pode integrar o Vault com outras ferramentas da Hashicorp como Consul ou Nomad. Em outras palavras, nos permite construir uma plataforma nativa da nuvem de forma segura. Para obter mais detalhes, consulte o artigo Secure Spring Cloud Microservices com Vault e Nomad.
- https://piotrminkowski.com/2021/05/24/ssl-with-spring-webflux-and-vault-pki/

## Subindo vault
```
docker run --cap-add=IPC_LOCK -d --name vault -p 8200:8200 vault
docker logs vault (pegar token de acesso)
```
