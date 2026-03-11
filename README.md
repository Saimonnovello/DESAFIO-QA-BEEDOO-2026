# DESAFIO-QA-BEEDOO-2026

Qual você acredita ser o objetivo da aplicação?
- Acredito que seja sobre cadastrar cursos e gerenciar

Quais são os principais fluxos disponíveis?
- É possivel cadastrar cursos.
- excluir e vizualizar.
- Pode cadastrar data, descrição, instrutor e outras informações.

Quais pontos do sistema você considera mais críticos para teste?
- Eu observei que na hora de excluir os cursos não exclui, aparece a mensagem ( excluido com sucesso ) mas não exclui.
- Outro ponto é no limite de palavras na hora de cadastrar um curso, não tem limite e fica desproporcional quando vai vizualizar o curso.
- Se cadastrar um curso sem titulo e outras informações, ele cadastra igual sem informações.
________________________________________________
Fluxo principal de cadastro de curso.
Cenário: Cadastro de curso

1. Abrir tela de cadastro de cursos
2. prencher nome do curso e outras informações
3. clicar em cadastrar curso

Resultado:
Curso cadastrado com sucesso
_________________________________________________
Listagem de cursos
Cenário: lista de cursos

1. Abrir tela de listar cursos

Resultado:
Deve mostrar os cursos cadastrados
__________________________________________________
Cenários negativos
Cenário: excluir curso

1. Entrar em listar cursos
2. Clicar em excluir curso

Resultado:
Deveria excluir o curso quando clicar em excluir

Cenário: Cadastrar curso sem nenhuma informação

1. entrar em cadastrar curso
2. Deixar vazio o nome e as informações
3. Clicar em cadastrar curso para salvar

Resultado:
Deveria mostrar uma mensagem de erro
___________________________________________________
Validações de campos
Cenario: validação de campos

1. Entrar em cadastrar cursos
2. prencher informações nos campos
3. clicar em cadastrar curso para salvar

Resultado:
sistema deve impedir o cadastro se estiver errado as informações nos campos como ( data, instrutor, tipo de curso, numero de vagas )
___________________________________________________
Comportamentos inesperados
Cenário: cursos desproporcional

1. Entrar em cadastrar curso
2. prencher informações com muitas palavras
3. clicar em cadastrar curso para salvar

Resultado:
os cursos ficam com tamnhos diferentes. Desproporcionais quando colocado muitas informações.
___________________________________________________

Registro de Bugs
Titulo: Curso duplicado

Passo a Passo
1. cadastrar um curso duas vezes com as mesmas informações
2. clicar em cadastrar curso para salvar

Resultado atual:
ele permite dois cursos duplicado

Resultado esperado:
deveria aparecer uma mensagem de erro quando cadastrar dois cursos duplicados

Severidade:
alta
____________________________________________________

link da planilha de casos e testes no Google planilha:
https://docs.google.com/spreadsheets/d/1frqqe0lMUA4dpg2pgF60NNVSaE-Qp-0ZYSkQbV5rIb4/edit?usp=sharing

link da execução dos testes:
https://drive.google.com/drive/folders/1L2HNZuGTmS03wHNcd6oDKh3hQNy-jus6?usp=sharing





