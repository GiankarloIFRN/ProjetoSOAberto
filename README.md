# Ferramenta de diagnóstico e auditoria de servidores Linux
Ferramenta de diagnóstico e auditoria de servidores Linux

Desenvolvimento de uma aplicação em Shell Script

1. Apresentação e contextualização
Imagine que uma empresa possui vários servidores Linux responsáveis por hospedar
aplicações, armazenar arquivos e fornecer serviços de rede. A equipe de infraestrutura precisa
verificar periodicamente se esses servidores estão funcionando corretamente.
Entre as atividades comuns estão:  Verificar se as interfaces de rede estão configuradas e ativas.  Conferir os endereços IP e as rotas configuradas.  Testar a conectividade com outros equipamentos.  Verificar se determinados serviços estão em execução.  Analisar registros de acesso e identificar erros.  Gerar relatórios de diagnóstico.  Registrar as verificações realizadas para consultas posteriores.
Atualmente, essas tarefas podem ser executadas manualmente, utilizando vários
comandos diferentes do Linux. O objetivo deste projeto é desenvolver um programa em Shell
Script que automatize parte dessas atividades, reunindo as verificações em uma única
ferramenta de linha de comando.

2. Objetivo do projeto
Desenvolver uma ferramenta chamada netadmin.sh, executada pelo terminal, que
receba opções e argumentos, realize verificações de diagnóstico e auditoria de um servidor Linux
e apresente os resultados de maneira organizada. O programa deverá ser modular, validar
entradas, tratar situações de erro e permitir a geração de relatórios.

3. Funcionamento esperado e interface de utilização
A ferramenta deverá aceitar opções que determinem quais operações serão realizadas.
Opção Finalidade -i Exibir informações do servidor e das interfaces de rede. -p DESTINO Testar a conectividade com um destino.
-P ARQUIVO Testar a conectividade com todos os destinos listados em um arquivo.
-s Listar serviços e portas em estado de escuta. -c PORTAS Verificar uma ou mais portas locais específicas (separadas por vírgula). -l ARQUIVO Analisar um arquivo de log. -o ARQUIVO Salvar os resultados em um relatório.
-v Ativar o modo detalhado.
-h Exibir a ajuda de utilização.

O programa deverá informar quando uma opção exigir um argumento e esse argumento
não tiver sido fornecido.
