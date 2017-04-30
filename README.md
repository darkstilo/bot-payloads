# Esqueletos GET

> GET http://clareando.claro.com.br/ HTTP/1.1[crlf]Host: clareando.claro.com.br[crlf][crlf]CONNECT [host_port] [protocol][crlf][crlf]
- [x] Texto de Conexão: Normal
- [x] Método Requisitado: GET
- [x] Método Injeção: Inicial
- [ ] Cabeçalhos Extras: Não

## Esqueletos Front Query

> GET http://clareando.claro.com.br/ HTTP/1.1[crlf]Host: clareando.claro.com.br[crlf][crlf]CONNECT clareando.claro.com.br@[host_port] [protocol][crlf][crlf]
- [x] Texto de Conexão: Normal
- [x] Método Requisitado: GET
- [x] Método Injeção: Inicial
- [x] Método de Consulta: Front Query
- [ ] Cabeçalhos Extras: Não

> GET http://clareando.claro.com.br/ HTTP/1.1[crlf]Host: clareando.claro.com.br[crlf]X-Online-Host: clareando.claro.com.br[crlf]X-Forward-Host: clareando.claro.com.br[crlf]X-Forwarded-For: clareando.claro.com.br[crlf]Connection: Keep-Alive[crlf]User-Agent: [ua][crlf][crlf]CONNECT clareando.claro.com.br@[host_port] [protocol][crlf][crlf]

- [x] Texto de Conexão: Normal
- [x] Método Requisitado: GET
- [x] Método Injeção: Inicial
- [x] Método de Consulta: Front Query
- [x] Cabeçalhos Extras: Sim

> GET http://clareando.claro.com.br/ HTTP/1.1[crlf]Host: clareando.claro.com.br[crlf]CONNECT [host_port] [protocol][crlf][crlf]CONNECT clareando.claro.com.br@[host_port] [protocol][crlf][crlf]

- [x] Texto de Conexão: Normal
- [x] Método Requisitado: GET
- [x] Método Injeção: Inicial
- [x] Método de Consulta: Front Query
- [ ] Cabeçalhos Extras: Não
- [x] Conexão Dupla: Sim

GET http://clareando.claro.com.br/ HTTP/1.1[crlf]Host: clareando.claro.com.br[crlf]X-Online-Host: clareando.claro.com.br[crlf]X-Forward-Host: clareando.claro.com.br[crlf]X-Forwarded-For: clareando.claro.com.br[crlf]Connection: Keep-Alive[crlf]User-Agent: [ua][crlf]CONNECT [host_port] [protocol][crlf][crlf]CONNECT clareando.claro.com.br@[host_port] [protocol][crlf][crlf]

- [x] Texto de Conexão: Normal
- [x] Método Requisitado: GET
- [x] Método Injeção: Inicial
- [x] Método de Consulta: Front Query
- [x] Cabeçalhos Extras: Sim
- [x] Conexão Dupla: Sim

## Esqueletos Back Query

> GET http://clareando.claro.com.br/ HTTP/1.1[crlf]Host: clareando.claro.com.br[crlf][crlf]CONNECT [host_port]@clareando.claro.com.br [protocol][crlf][crlf]

- [x] Texto de Conexão: Normal
- [x] Método Requisitado: GET
- [x] Método Injeção: Inicial
- [x] Método Consulta: Back Query
- [ ] Cabeçalhos Extras: Não

## Esqueleto Conexão Dupla

> GET http://clareando.claro.com.br/ HTTP/1.1[crlf]Host: clareando.claro.com.br[crlf]CONNECT [host_port] [protocol][crlf][crlf]CONNECT [host_port] [protocol][crlf][crlf]

- [x] Texto de Conexão: Normal
- [x] Método Requisitado: GET
- [x] Método Injeção: Inicial
- [x] Extra: Conexão Dupla
- [ ] Cabeçalhos Extras: Não
