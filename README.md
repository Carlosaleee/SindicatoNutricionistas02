 Atividade 02 - Uc9 - Senac ead - Tecnico em Desenvolvimento de Sistemas

 
Contexto
O Sindicato dos Nutricionistas pretende fazer uma ação diferente com seus associados. Ele distribuirá aos nutricionistas softwares desktop para realizar rapidamente cálculos muito comuns na rotina desses profissionais.
 
O software precisa realizar:
 
Cálculo de IMC (índice de massa corporal)
Calculo de gasto calórico basal, que é quanto uma pessoa gasta de caloria para simplesmente sobreviver
Cálculo de gasto calórico total, que considera a quantidade de atividades físicas que a pessoa realiza
Recomendação de quantidade de carboidrato, proteína e gordura que a pessoa deve ingerir
 
Atividade
Crie um projeto Java no NetBeans e implemente as seguintes funcionalidade e telas usando a ferramenta visual do IDE (ambiente de desenvolvimento integrado, em inglês integrated development environment).
 
Crie uma tela inicial baseada no wireframe a seguir. Ela será a tela que deve abrir ao executar o programa e, ao clicar nos botões, levar às telas seguintes.

Descrição: Wireframe de uma tela com três botões ao centro, alinhados verticalmente: “IMC”, “Gasto Calórico” e “Recomendações”.Clique para obter mais opções
 Figura 1 – IMC, gasto calórico e recomendações
Fonte: Senac EAD (2022)
 
Crie a tela IMC baseando-se no seguinte wireframe.
 

Descrição: Wireframe da tela com título “Cálculo de IMC”, um painel com o rótulo “Altura (m)”, seguido de um campo de entrada de texto à direita. Abaixo, há o rótulo “Peso (kg)”, seguido de um campo de entrada e, mais abaixo, um botão “Calcular”. Ainda mais abaixo, há um painel com os rótulos “Resultado” e “Interpretação”.
Figura 2 – Cálculo de IMC
Fonte: Senac EAD (2022)
 
Essa tela será acessada por meio do botão IMC da tela principal e deverá aparecer sobre ela (não por trás).
 
Ao clicar em Calcular, o programa deve coletar os dados informados e realizar a operação “IMC = Peso / Altura²”. O resultado dessa operação aparecerá após o label Resultado. À direita do label Interpretação, deve conter um dos seguintes textos:
 
“Magreza”, se o IMC for menor que 18,5
“Normal”, se o IMC for entre 18,5 e 24,9
“Sobrepeso”, se o IMC for entre 25 e 29,9
“Obesidade”, se o IMC for entre 30 e 39,9
“Obesidade grave”, se o IMC for maior ou igual a 40
 
Essa tela será acessada por meio do botão IMC da tela principal e deverá aparecer sobre ela (não por trás).
 
Validações: a tela não deve “quebrar” ao informar valores inválidos; a tela deve solicitar que o usuário preencha todos os campos.
 
Crie a tela Gasto Calórico baseando-se no seguinte wireframe.
 

Descrição: Wireframe de uma tela com o título “Cálculo de Gasto Calórico” e, abaixo, um painel contendo dois radio buttons com o rótulo “Mulher” e “Homem” desmarcados. Abaixo, há um rótulo “Peso (kg)”, seguido, à direita, de um campo de entrada de texto. Abaixo, há um rótulo “Altura (cm)”, seguido, à direita, de um campo de entrada de texto. Abaixo, há um rótulo “Idade”, seguido, à direita, de um campo de entrada de texto. Abaixo, há um rótulo “Nível de atividade”, seguido, à direita, de um campo de seleção. Ainda mais abaixo, há um segundo painel com os rótulos “Gasto Basal” e “Gasto Total”. Clique para obter mais opções
Figura 3 – Cálculo de gasto calórico
Fonte: Senac EAD (2022)
 
Essa tela será acessada por meio do botão Gasto Calórico da tela principal.
 
Ao clicar em Calcular, o programa deve, primeiro, realizar o cálculo de gasto calórico basal, que varia de acordo com o sexo da pessoa:
 
Homem
Mulher
CalBasal = 66 + (13,8 * Peso) + (5 * Altura) – (6,8 * Idade)
CalBasal = 655 + (9,6 * Peso) + (1,9 * Altura) – (4,7 * Idade)
 
Esse valor deve aparecer à direita do label Gasto Basal na tela.
 
Depois disso, com base no gasto de caloria basal obtido pelo cálculo anterior, deve-se calcular o gasto total, que varia de acordo com o nível de atividade física da pessoa:
 
Nível de atividade
Cálculo
Sedentário
calTotal = CalBasal * 1,2
Leve (exercício leve 1 a 3 dias/semana)
calTotal = CalBasal * 1,375
Moderado (exercício moderado 3 a 5 dias/semana)
calTotal = CalBasal * 1,55
Ativo (exercício pesado 5 a 6 dias/semana)
calTotal = CalBasal * 1,725
Extremamente ativo (exercício pesado diário)
calTotal = CalBasal * 1,9
 
A combobox presente na tela deve oferecer as opções listadas anteriormente para “nível de atividade”.
 
O valor obtido pelo cálculo deve aparecer à direita do label Gasto Total.
 
Validações: a tela não deve “quebrar” ao informar valores inválidos; a tela deve solicitar que o usuário preencha todos os campos.
 
Crie a tela Recomendações baseando-se no wireframe a seguir.
 

Descrição: Wireframe de tela com o título “Recomendações” e um painel contendo um rótulo “Calorias diárias (kcal)”, seguido, à direita, de um campo de entrada de texto. Abaixo, há um botão “Calcular”. Abaixo, outro painel com os rótulos “Carboidratos (50%)”, “Proteína (25%)” e “Gordura (25%)”.Clique para obter mais opções
 Figura 4 – Recomendações
Fonte: Senac EAD (2022)
 
Essa tela será acessada por meio do botão Recomendações da tela principal.
 
Ao clicar em Calcular, o programa deve usar a quantidade de calorias informada e calcular, da seguinte maneira, a quantidade recomendada dos nutrientes:
 
Carboidratos = calorias * 0,5 / 4
Proteínas = calorias * 0,25 / 4
Gordura = calorias * 0,25 / 9
 
Os resultados devem aparecer à direita dos componentes de label correspondentes e devem ser expressos em gramas (g).
 
Observação: nas três últimas telas, implemente as seguintes validações: o programa não deve “quebrar” ao informar valores inválidos, mas, sim, mostrar uma mensagem amigável ao usuário; a tela deve solicitar que o usuário preencha todos os campos antes de realizar o cálculo.
 
Entrega
No espaço dedicado às entregas da atividade, envie um arquivo compactado (ZIP, RAR ou 7z) contendo todos os projetos NetBeans criados para esta.
 
Dica de leitura
Para esta atividade, leia os seguintes materiais:
 
Interface desktop: construção de interface de usuário, manipulação de eventos, uso de controles, manipulação de janelas, construção de formulários e listagens (parte 1)
Interface desktop: construção de interface de usuário, manipulação de eventos, uso de controles, manipulação de janelas, construção de formulários e listagens (parte 2)
Validações de formulário: funções da linguagem, formatação de dados
Tratamento de exceções em linguagem de programação: comandos, classes, aplicabilidade
 
Avaliação
Nesta atividade, você será avaliado no seguinte indicador:
 
Elabora interface gráfica de acordo com requisitos do sistema e considerando tendências de mercado. 
