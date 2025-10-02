Filtragem de Dados em Relatórios

Contexto: um sistema gera relatórios que podem ser filtrados por diferentes critérios (por data, por usuário, por status, por valor).

Atividade: implemente FilterStrategy e permita ao usuário aplicar filtros diferentes sem alterar a lógica central de geração do relatório.

---
# Filtragem Dinâmica
No Sistema de Cadastros da [ONG Amor Em Movimento](), existe uma filtragem de dados, para os Voluntários encontrarem o cadastro correto.

Há uma série de combinações possíveis para filtrar os dados, combinando os diferentes itens de pesquisa:
- Nome,
- Data de Nascimento,
- Tamanho do Calçado,
- Tamanho da Roupa.

Afim de evitar utilizar, excessivamente, Condições Lógicas para montar as queries corretamente, e responder com o retorno esperado pelo usuário, foi idealizada a implementação do Design Pattern Strategy, que irá auxiliar no reaproveitamento de comportamento dos Filtros, aplicando para o contexto adequado, aplicado nos filtros.

