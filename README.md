# 💳 Projeto Conta Bancária  

Este repositório contém um sistema de **conta bancária** desenvolvido para demonstrar as operações financeiras básicas em uma conta. O projeto permite realizar operações de **depósito**, **saque**, **transferência** e **consulta de saldo**.

🚀 **Tecnologias utilizadas**:  
![Java](https://img.shields.io/badge/Java-007396?style=flat&logo=java&logoColor=white)  
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat&logo=spring-boot&logoColor=white)  

---

## 📌 Funcionalidades  

- **Cadastro de Conta**: Criação de uma nova conta bancária.
- **Depósito**: Realização de depósitos em uma conta.
- **Saque**: Saques realizados diretamente na conta.
- **Transferência**: Transferências entre contas.
- **Consulta de Saldo**: Verificação do saldo da conta bancária.

---

## 🚀 Como Executar  

1. **Clone o repositório**  
```bash
git clone https://github.com/sandramastrogiacomo/contabancaria.git
cd contabancaria
Compile e execute a aplicação

bash
Copiar
Editar
mvn clean install
mvn spring-boot:run
A aplicação estará disponível em http://localhost:8080.

📡 Testes com Insomnia
Os testes da API foram realizados utilizando Insomnia. Aqui estão alguns exemplos de requisições que podem ser feitas para testar as funcionalidades do sistema:

Cadastrar Conta
POST http://localhost:8080/conta/cadastrar
Corpo da requisição:

json
Copiar
Editar
{
  "nome": "João da Silva",
  "agencia": "1234",
  "conta": "987654",
  "saldo": 1000.00
}
Depósito
POST http://localhost:8080/conta/deposito
Corpo da requisição:

json
Copiar
Editar
{
  "contaId": 1,
  "valor": 500.00
}
Saque
POST http://localhost:8080/conta/saque
Corpo da requisição:

json
Copiar
Editar
{
  "contaId": 1,
  "valor": 200.00
}
Transferência
POST http://localhost:8080/conta/transferir
Corpo da requisição:

json
Copiar
Editar
{
  "contaOrigemId": 1,
  "contaDestinoId": 2,
  "valor": 150.00
}
Consultar Saldo
GET http://localhost:8080/conta/{id}/saldo

Substitua {id} pelo ID da conta para consultar o saldo.

🤝 Contribuições
💡 Contribuições são bem-vindas! Se tiver sugestões, melhorias ou encontrar problemas, abra uma issue ou envie um pull request.

📜 Licença
📝 Este projeto está licenciado sob a MIT License.

📬 Contato
🔗 GitHub: sandramastrogiacomo
🔗 LinkedIn: Sandra Mastrogiacomo

📌 Este projeto foi desenvolvido para demonstrar operações bancárias básicas com Java e Spring Boot.
