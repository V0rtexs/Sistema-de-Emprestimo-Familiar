Sistema de Controle de Empréstimos Familiares (C# Console)

Este projeto é uma aplicação de console desenvolvida em C# para gerenciar empréstimos financeiros entre membros de uma família. O foco principal é garantir a transparência e a integridade das operações através de assinaturas digitais (senhas) e cálculos automáticos de reajuste financeiro.

🚀 Funcionalidades Principais

-Gestão de Usuários: Cadastro de familiares com nomes imutáveis para garantir a integridade dos registros.

-Registro de Empréstimos: Cadastro detalhado contendo data, credor, devedor e valor original.

-Cálculo Automático de Reajuste: O sistema aplica juros compostos de 0,1% ao dia sobre o valor original.

-Aplicação de Multas: Incidência de multa de 10% a cada 30 dias sobre o valor já atualizado.

-Relatórios Filtráveis: Visualização do extrato de dívidas com opção de filtro por nome do credor ou devedor.

-Painel Administrativo: Permite que um administrador altere as taxas de juros e multas dinamicamente.

⚖️ Regras de Negócio e Segurança

-Assinatura Digital: Nenhuma operação é realizada sem validação. O devedor deve assinar (senha) a criação do empréstimo e o credor deve assinar a quitação.

-Integridade dos Dados: Não é permitida a alteração de informações de um empréstimo após o registro.

-Privacidade e Limpeza: O sistema não mantém registros de empréstimos quitados; após o pagamento confirmado, a dívida é excluída da lista ativa.

-Validação de Fluxo: O sistema possui tratamento de erros que permite ao usuário corrigir entradas inválidas sem perder o progresso da operação atual.

🛠️ Conceitos de Engenharia de Software Aplicados

O sistema foi construído seguindo contratos de responsabilidade específicos para garantir a modularidade:

-ObtemListaDeEmprestimo: Lógica de filtragem e recuperação de dados.

-ObtemValorReajustado: Motor de cálculo financeiro.

-ConfirmaOPagamento: Protocolo de segurança e exclusão de registros.

💻 Tecnologias Utilizadas

-C# (.NET)

-LINQ (para filtragem de dados)

-Console Application
