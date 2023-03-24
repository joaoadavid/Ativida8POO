# Ativida8POO
# OrientadaObjetos3
Atividade 3
### Classes:

- Cliente
- Conta Bancária
- Transação Bancária
- TransferenciaQR

### Atributos:

**Cliente:**

- Nome completo: String
- CPF: String
- Data de nascimento: Date

**ContaBancaria (herda de Cliente):**

- Número da conta: String
- Nome do titular: String
- Saldo: Double

**Transação Bancária:** 

- Valor da transação: Double
- Data: Date
- Conta de origem: ContaBancaria
- Conta de destino: ContaBancaria
- Tipo de transação (depósito, saque ou transferência)

**TransferênciaQR:** 

- QR Code: String
- Informações da conta bancária (atrelado ao QR Code)

### Métodos:

**Cliente:**

- Criar conta bancária

**Conta Bancária:**

- Verificar saldo
- Solicitar operação (saque, deposito e transferencia)
- Consultar informações da operação

**Transação Bancária:**

- Realizar operação (saque, deposito e transferencia)
- Registrar e guardar informações da operação

**TransferenciaQR:**

- Gerar um QR Code por Conta Bancária
- Escanear QR Code da Conta Bancária
- Solicitar operação (saque, deposito e transferencia) usando o QR Code como identificação

### **Relacionamentos:**

*Cada Cliente pode ter uma ou mais Contas Bancárias. (1 : N) 
Cada Conta Bancária pertence a um único Cliente. (N : 1)
Cada Transação Bancária envolve duas Contas Bancárias. (2:2)
Cada Conta Bancária pode ter várias Transações Bancárias. (1 : N)
A TransferênciaQR interage com as Contas Bancárias dos Clientes e solicita Transações Bancárias.*
