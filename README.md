# Sistema de Gerenciamento de Ordens de Serviço - Oficina Mecânica

Este projeto visa modelar o esquema conceitual de um sistema para controle e gerenciamento de ordens de serviço (OS) em uma oficina mecânica.

## Objetivo

Criar um esquema conceitual que represente o contexto de uma oficina mecânica, onde clientes levam seus veículos para reparos e revisões. O sistema deve permitir o gerenciamento de clientes, veículos, mecânicos, serviços, peças e ordens de serviço.

## Narrativa

O sistema deve abranger os seguintes aspectos:

* **Clientes** levam **veículos** à oficina para reparos ou revisões periódicas.
* Cada **veículo** é designado a uma **equipe de mecânicos** que identifica os serviços a serem executados e preenche uma **OS** com a data de entrega.
* O valor de cada **serviço** é calculado com base em uma tabela de referência de mão de obra.
* O valor das **peças** utilizadas também compõe a OS.
* O **cliente** autoriza a execução dos serviços.
* A mesma equipe de **mecânicos** avalia e executa os serviços.
* Os **mecânicos** possuem código, nome, endereço e especialidade.
* Cada **OS** possui número, data de emissão, valor, status e data de conclusão.

## Esquema Conceitual

O esquema conceitual foi modelado utilizando o Diagrama Entidade-Relacionamento (DER) e está disponível no arquivo 'esquema_conceitual.md'.

## Entidades e Atributos Principais

* **Cliente**:
    * Nome
    * Endereço
    * CPF
    * Telefone
* **Veículo**:
    * Placa
    * Modelo
    * Marca
    * Ano
* **Mecânico**:
    * Código
    * Nome
    * Endereço
    * Especialidade
* **Serviço**:
    * Código
    * Descrição
    * Valor da Mão de Obra
* **Peça**:
    * Código
    * Nome
    * Descrição
    * Valor Unitário
* **OS (Ordem de Serviço)**:
    * Número
    * Data de Emissão
    * Data de Conclusão
    * Status (Aberta, Em Andamento, Concluída)
    * Valor Total

## Relacionamentos

* Um Cliente possui um ou mais Veículos.
* Um Veículo possui uma ou mais Ordens de Serviço.
* Uma Ordem de Serviço é designada a um ou mais Mecânicos.
* Uma Ordem de Serviço contém um ou mais Serviços.
* Uma Ordem de Serviço contém uma ou mais Peças.

## Próximos Passos

* Implementar o esquema lógico do banco de dados.
* Desenvolver a aplicação para gerenciamento das ordens de serviço.

# desafio.dio
Esquema Conceitual para Banco de Dados
