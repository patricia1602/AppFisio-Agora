### PROJETO INTEGRADOR: ANÁLISE DE SOLUÇÕES INTEGRADAS PARA ORGANIZAÇÕE

## Fisio-Agora  

## 👨‍💻 Desenvolvido por

Grupo 03 — Projeto Integrador 2 
Turma 2501 — Curso de Análise e Desenvolvimento de Sistemas 
**Orientador**: Prof. Carlos Henrique Veríssimo Pereira  
**Tutora**: Ruth Garcia 

**Integrantes:**  
- Jacqueline Rodrigues Oliveira  
- Nathan da Silva Rocha  
- Patricia Costa da Silva Souza  
- Pedro Ivo Maldonado Roschel  
- Vinicius Cardoso Meira  

# 🩺 Fisio Agora!

O **Fisio Agora!** é um sistema desenvolvido para facilitar o acesso de pacientes a atendimentos fisioterapêuticos, conectando-os a fisioterapeutas e estagiários por meio de instituições parceiras. Este repositório contém os diagramas fundamentais para o entendimento da estrutura de dados e das funcionalidades da aplicação.

---

## 📊 Diagrama de Entidade e Relacionamento (DER)

O **DER** apresenta as principais entidades do sistema e seus relacionamentos.

### ✅ Entidades Principais

- **Paciente**: nome, data de nascimento, CPF, telefone, e-mail, endereço  
- **Fisioterapeuta**: nome, registro profissional, especialidade, telefone, e-mail, endereço  
- **Especialidade**: nome da especialidade e descrição  
- **Consulta**: associa paciente, fisioterapeuta, data, hora e status  
- **Agendamento**: data, hora, paciente, fisioterapeuta, status  
- **Instituição Parceira**: nome, telefone, e-mail e endereço  
- **Estudante**: nome, matrícula, instituição vinculada  
- **Usuário**: login de acesso como paciente ou fisioterapeuta  
- **Admin**: gerenciamento de especialidades, instituições e usuários  
- **Endereço**: compartilhado entre entidades que precisam de localização

### 🔗 Principais Relacionamentos

- Paciente ↔ Agendamento: 1-N  
- Fisioterapeuta ↔ Agendamento: 1-N  
- Agendamento → Consulta: 1-1  
- Consulta → Instituição: N-1  
- Fisioterapeuta → Especialidade: N-1  
- Estudante → Instituição: N-1  
- Usuário ↔ Paciente/Fisioterapeuta: 1-1  
- Endereço compartilhado entre várias entidades

### 📷 Imagem do DER

![Diagrama DER](assets/diagrama_der.png)

---

## 🎭 Diagrama de Casos de Uso

O diagrama de casos de uso representa como os diferentes **atores do sistema** interagem com suas respectivas funcionalidades.

### 👥 Atores

- **Paciente**: agendamentos, histórico, perfil  
- **Fisioterapeuta**: agenda, consultas, perfil  
- **Estudante**: registro e histórico de atendimentos  
- **Admin**: gerenciamento de especialidades, instituições e usuários  
- **Instituição Parceira**: histórico de consultas

### 🧩 Casos de Uso

- Realizar agendamento  
- Consultar histórico de consultas  
- Registrar atendimento  
- Acessar perfil  
- Gerenciar especialidades  
- Gerenciar instituições parceiras  
- Acessar agenda  
- Gerenciar usuários  
- Realizar login e cadastro

### 📷 Imagem do Diagrama de Casos de Uso

![Diagrama de Casos de Uso](./assets/diagrama_casos_de_uso.png)

---

## 🚀 Tecnologias e Ferramentas

- JavaScript, HTML, CSS  
- React Native com Expo  
- Banco de dados relacional (DER)  
- UML para modelagem de casos de uso  
- Figma para prototipação

---







