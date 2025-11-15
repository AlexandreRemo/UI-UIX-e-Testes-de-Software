# UI-UIX-e-Testes-de-Software
Matéria UI/UIX
Cálculo da Complexidade Ciclomática do método CONECTAR BD

 Identificação das decisões

O método possui um bloco try-catch.

O catch representa uma decisão, pois existem dois caminhos possíveis:

Execução normal do try

Execução do catch em caso de exceção

Passo 2: Aplicação da fórmula
Fórmula:
V(G)=numero de decisoes+1
Número de decisões = 1 (catch)
𝑉(𝐺)=1+1=2
V(G)=1+1=2

Conclusão:
A complexidade ciclomática do método conectarBD() é 2.

Isso indica que existem 2 caminhos independentes: sucesso ou exceção.


CALCULO DE CAMINHOS BÁSICOS DO MÉTODO ConectarBD()

Passo 1: Listar os possíveis fluxos

Caminho 1 – Sucesso

Fluxo: execução do try sem erro

Resultado esperado: conexão retornada não-nula

Caminho 2 – Exceção

Fluxo: exceção é capturada no catch

Resultado esperado: método retorna null

Conclusão:

Número de caminhos básicos = 2, igual à complexidade ciclomática.

Cada caminho independente deve ser testado em um caso de teste.


Cálculo da Complexidade Ciclomática
if (rs.next()) → 1 decisão
Bloco try-catch → 1 decisão implícita (exceção)
Número de decisões = 2
V(G)=numero de decisoes+1=2+1=3
A complexidade ciclomática do método verificarUsuario() é 3.
Existem 3 caminhos independentes: usuário encontrado, usuário não encontrado, exceção.


CAMINHOS BÁSICOS

Caminho A – Usuário encontrado

Condição: rs.next() retorna true

Resultado esperado: result = true e nome preenchido

Caminho B – Usuário não encontrado

Condição: rs.next() retorna false

Resultado esperado: result = false e nome não preenchido


Caminho C – Exceção durante conexão ou execução da consulta

Condição: erro no try (conexão ou execução da query)

Resultado esperado: result = false e nome não preenchido

Número de caminhos básicos = 3, igual à complexidade ciclomática

Conclusão:

Cada caminho representa um fluxo independente que deve ser testado.

Método	            Decisões	Complexidade Ciclomática	Caminhos Básicos	Descrição dos Caminhos
conectarBD()	        1	             2	                        2	             1.Sucesso / 2. Exceção
verificarUsuario()	  2	              3	                        3	             1. Usuário encontrado / 2. Usuário não                                                                                         encontrado / 3. Exceção
