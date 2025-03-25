
# 🩺 Análise e Projeto de Sistema - Clínica Médica

## 📌 Sobre

Repositório voltado para a formulação de um sistema proposto durante as aulas de APS 2025.1. Aqui você poderá encontrar desde diagramas de casos de uso, de entidade e relacionamento, até o levantamento de requisitos de um complexo direcionado ao funcionamento de uma clínica médica.

---
## 📅 Cronograma do Projeto

| Data        | Descrição                             |
|-------------|---------------------------------------|
| 11/03/2025  | Levantamento de Requisitos            |
| 18/03/2025  | Diagrama de casos de uso              |
| 25/03/2025  | Diagrama de entidade e relacionamento |

---

## ✔️ Requisitos Funcionais

#### 1. Agendamento de Consultas – O sistema deve permitir que pacientes marquem, remarquem e cancelem consultas online (Permanente, Evidente e Obrigatório). 
#### 2. Cadastro de Pacientes – O sistema deve permitir o registro de novos pacientes, armazenando dados pessoais e históricos médicos (Permanente, Evidente e Obrigatório).
#### 3. Prontuário Eletrônico – O sistema deve permitir que médicos acessem e atualizem prontuários dos pacientes de forma segura (Permanente, Evidente e Obrigatório).
#### 4. Emissão de Receitas e Atestados – O sistema deve possibilitar que médicos gerem e imprimam receitas médicas e atestados para os pacientes  (Permanente, Evidente e Obrigatório).
#### 5. Notificações e Lembretes – O sistema deve enviar notificações automáticas para lembrar pacientes sobre consultas agendadas (Permanente, Oculto e Desejado).
#### 6. Gerenciamento de Pagamentos – O sistema deve permitir o controle de pagamentos, emissão de faturas e integração com meios de pagamento eletrônico (Permanente, Evidente e Obrigatório).
#### 7. Controle de Estoque de Medicamentos – O sistema deve permitir o gerenciamento do estoque de insumos e medicamentos da clínica. (Permanente, Oculto e Desejado).
#### 8. Relatórios e Estatísticas – O sistema deve gerar relatórios sobre atendimentos, ocupação de agenda e faturamento (Transitório, Oculto e Desejado).

---

## 📋 Requisitos Não Funcionais

#### 1. Segurança dos Dados – o sistema deve garantir que os dados dos pacientes sejam armazenados e transmitidos de forma segura

#### 2. Desempenho – o sistema deve ser capaz de processar pelo menos x agendamentos simultâneos sem perda de desempenho

#### 3. Usabilidade – interface intuitiva e acessível para usuários

---

## 📜 A Extensão dos Requisitos

#### 1.E - Cancelamento automático de Consultas 

Descrição: *O sistema deve permitir o cancelamento automático de consultas caso o paciente não confirme a presença dentro de um período pré-determinado. O paciente recebe um lembrete via SMS ou e-mail e deve confirmar a consulta. Caso não haja resposta dentro do tempo estipulado, a consulta será cancelada e disponibilizada para outro paciente.*

Fontes: (gerente da clínica) e regulamento interno de agendamentos.

Usuário: Pacientes e recepcionistas.

Informações de entrada: Código da consulta e confirmação do paciente (Sim/Não).

Informações de saída: Status atualizado da consulta (Confirmada ou Cancelada) e notificação ao paciente e recepcionista.

Restrições lógicas: O cancelamento automático só ocorre se o paciente não confirmar até X horas antes do horário agendado.

Restrições tecnológicas: O sistema deve estar integrado a uma ferramenta de envio de SMS e e-mail.
                       
#### 3.E - Histórico de alterações no Prontuário

Descrição: *O sistema deve registrar um histórico de todas as modificações realizadas nos prontuários eletrônicos dos pacientes. 
Cada alteração deve incluir informações como data, hora, usuário responsável e o que foi alterado, garantindo a rastreabilidade e conformidade com normas médicas.*

Fontes: Doutor X

Usuário: Médicos e administradores da clínica.

Informações de entrada: Identificação do prontuário, detalhes da alteração e usuário que realizou a modificação.

Informações de saída: Relatório com histórico de edições no prontuário, contendo data, hora e usuário responsável.

Restrições lógicas: Apenas usuários autorizados podem visualizar o histórico completo.

Restrições tecnológicas: O sistema deve garantir integridade e segurança das 
informações 

#### 6.E - Parcelamento

Descrição: O sistema deve permitir que pacientes optem por parcelar pagamentos de consultas e procedimentos médicos. O parcelamento poderá ser feito via cartão de crédito ou boleto bancário, de acordo com as regras definidas pela clínica.

Fontes: Manual de pagamento

Usuário: Pacientes e setor financeiro da clínica.

Informações de entrada: Valor total do pagamento, número de parcelas desejado e método de pagamento.

Informações de saída: Confirmação do pagamento parcelado e fatura gerada com os detalhes das parcelas.

Restrições lógicas: Parcelamento disponível apenas para valores acima de x e limitado a y vezes sem juros

Restrições tecnológicas: O sistema deve estar integrado a um gateway de pagamento compatível com cartões e boletos bancários.

---

## 📊 Diagramas

#### [Visualizar Modelo de Entidade e Relacionamento](https://app.brmodeloweb.com/#!/publicview/67e29315d09ca118784afc3d)

#### [Visualizar Modelo de Casos de Uso](https://drive.google.com/file/d/1iYy7CG7j_m1HkgXq7BW8yuzClHA0EfP-/view?usp=sharing)
