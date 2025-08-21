# 📦 Projeto de Modelagem Conceitual – Oficina Mecânica  

## 📝 Descrição  
Este projeto apresenta a modelagem conceitual de um sistema de **gestão de oficina mecânica**, contemplando as principais entidades e relacionamentos que suportam o processo de atendimento ao cliente, manutenção de veículos, emissão de ordens de serviço, controle de equipes, serviços e peças utilizadas.  

O modelo foi elaborado para garantir **consistência e flexibilidade** no gerenciamento das informações da oficina, desde o cadastro de clientes até a conclusão do serviço prestado.  

---

## 🎯 Regras de Negócio Implementadas  

### Clientes e Veículos  
- Cada cliente pode possuir **um ou mais veículos** cadastrados.  
- Um veículo está sempre vinculado a um único cliente.  

### Ordens de Serviço  
- Cada veículo pode gerar diversas ordens de serviço.  
- Uma ordem de serviço possui informações como **datas, orçamento e status**.  
- Ordens de serviço estão ligadas a **equipes de mecânicos**.  

### Mecânicos e Equipes  
- Um mecânico pode participar de **mais de uma equipe**.  
- Cada equipe pode executar diversas ordens de serviço.  

### Serviços  
- Cada ordem de serviço pode envolver **vários serviços**.  
- Um serviço possui valor de mão de obra associado.  

### Peças  
- Cada serviço pode exigir **uma ou mais peças**.  
- O valor da peça é controlado para compor o orçamento final da ordem de serviço.  

---

## 📊 Estrutura Conceitual  

- **Cliente**: Nome, CPF, Contato, Endereço.  
- **Veículo**: Modelo, Placa, Ano, vínculo com Cliente.  
- **Ordem de Serviço**: Data de emissão, Data de conclusão, Orçamento, Status.  
- **Equipe**: Código da equipe, vínculo com mecânicos.  
- **Mecânico**: Nome, Código de identificação, Endereço, Especialidade.  
- **Serviço**: Descrição, Valor da mão de obra.  
- **Peça**: Descrição, Valor da peça.  
- **Controle de Ordens e Peças**: Relacionamentos que permitem associar múltiplos serviços e peças a cada ordem de serviço.  

---

## ✅ Conclusão  
O modelo conceitual da **Oficina Mecânica** atende aos requisitos principais:  

- Associação de clientes e veículos.  
- Gestão de ordens de serviço com status, orçamento e histórico.  
- Controle de equipes de mecânicos.  
- Registro detalhado de serviços e peças aplicadas.  

Este esquema fornece uma base sólida para a futura implementação do **banco de dados da oficina**.  

---

## 🖼️ Diagrama  
![Diagrama da Oficina](Oficina%20ABR3U's.png)  