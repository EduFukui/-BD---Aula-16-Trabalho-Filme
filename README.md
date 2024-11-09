# BD-Aula-16-Trabalho-Filme
# Descrição:
Armazenar as informações do filme

# Estrutura do Banco de Dados:
## Tabela: 
Personagem,
relacao,
contexto_sociocultural,
tratamento,
familia e
membrofamilia_tem
## Descrição: 
Armazenar as informações do usuario
## Colunas: 
Tabela: Personagem
- 'id_personagem' Identificador unico do personagem
- 'fk_tratamento_id_tratamento' Chave estrangeira de outra tabela chamada 'tratamento'
- 'fk_relacao_id_relacao' Chave estrangeira de outra tabela chamada 'relacao'
- 'nome_personagem' Nome do personagem
- 'idade' Idade do personagem
- 'etnia_personagem' Diz o tom de melatonina do personagem
- 'personalidade' Descreve a personalidade do personagem
- 'profissao' Diz qual o trabalho do personagem
- 'conflito' Descreve um conflito do personagem
- 'genero' Fala qual é o genero do personagem

Tabela: Relacao
- 'id_relacao' Identificador unico da relacao
- 'tipo_de_relacao' Descreve qual o tipo da relacao

Tabela: Familia
- 'id_familia' Identificador unico da familia
- 'nome-familia' Nome da Familia
- 'descricao_familia' Descreve a familia

Tabela: Contexto_sociocultural
-'id_contexto_sociocultural'  Identificador unico do contexto sociocultural
-'fk_familia_id_familia' Chave estrangeira da familia
-'fk_personagem_id_personagem' Chave estrangeira do personagem
-'lugar' Diz o local onde a familia/personagem moram
-'classe_social' Diz a condição da familia/personagem
-'etnia_contexto_sociocultural'  Diz o tom de melatonina da familia/personagem
-'cultura' Diz a cultura da familia/personagem

Tabela: Tratamento
-'id_tratamento'  Identificador unico do tratamento
-'descricao' Descreve o tratamento
-'nome_tratamento' Diz o nome do tratamento

Tabela: Membrofamilia_tem
-'fk_personagem_id_personagem' Chave estrangeira do personagem
-'fk_familia_id_familia' Chave estrangeira da familia
-'parentesco' Diz o parentesco de um personagem com um outro
-funcao' Diz a funcao de um personagem da familia

#Diagrama ER:
<img width="490" alt="Captura de tela 2024-11-08 215325" src="https://github.com/user-attachments/assets/868b09f5-4ed6-437a-9320-f7fac0dda425">
