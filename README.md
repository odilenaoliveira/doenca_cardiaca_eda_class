# doenca_cardiaca_eda_class
 visualização e classificação de doença cardiovascular

# Sobre o Conjunto de Dados

- O conjunto de dados se refere a mortalidade por doença cardíaca/ataque cardíaco, os dados contêm o histórico completo do status de vida dos pacientes, idade, sexo, fumante ou não fumante, se tem diabetes, colesterol, entre outras. O conjunto pede para criar um modelo que preveja a morte por insuficiência cardíaca.
- Mas, primeiro o conjunto de dados vai passar por um EDA, assim veremos as relações entre as colunas, qual paciente por gênero é mais afetado, qual a idade mais frequente, entre outros. Em seguida, irei criar modelos para a previsão e escolher o melhor resultado de acurácia do modelo.

- HEMOGLOBINA: uma proteína encontrada nas hemácias do sangue, este dá a coloração vermelha ao sangue e liga-se as moléculas de oxigênio para transportá-las pelo organismo. Valores de referência:
  - Masculino:
    - Idade 0-2 anos: Limite inferior (9,0), Limite Superior (14,7)
    - Idade 2-6 anos: Limite inferior (11,21), Limite Superior (14,1)
    - Idade 6-18 anos: Limite inferior (11,1), Limite Superior (14,0)
    - Idade 18-59 anos Limite inferior (13,1), Limite Superior (16,9)
    - Idade 60-mais anos: Limite inferior (12,4), Limite Superior (16,8)
  - Feminino:
    - Idade 0-2 anos: Limite inferior (9,0), Limite Superior (14,7)
    - Idade 2-6 anos: Limite inferior (3,5), Limite Superior (14,1)
    - Idade 6-18 anos: Limite inferior (3,93), Limite Superior (14,0)
    - Idade 18-59 anos Limite inferior (3,9), Limite Superior (14,8)
    - Idade 60-mais anos: Limite inferior (3,8), Limite Superior (15,1)

* **Uma baixa concentração de hemoglobina**, de acordo com outras características clínicas do indivíduo, pode sugerir gravidez, anemia por deficiência de ferro, anemia megaloblástica, talassemia, câncer, desnutrição, doença hepática ou lúpus.
* **Um aumento de hemoglobina** pode ser associado a policitemia, insuficiência cardíaca, doenças pulmonares e deslocamento para altitudes elevadas.
---
- VCM: indica o tamanho médio das hemácias
Valores de referência:
  - Masculino:
    - Idade 0-2 anos: Limite inferior (68), Limite Superior (137)
    - Idade 2-6 anos: Limite inferior (72), Limite Superior (88)
    - Idade 6-18 anos: Limite inferior (71), Limite Superior (99)
    - Idade 18-59 anos Limite inferior (81,5), Limite Superior (100,2)
    - Idade 60-mais anos: Limite inferior (86,3), Limite Superior (101,8)
  - Feminino:
    - Idade 0-2 anos: Limite inferior (68), Limite Superior (137)
    - Idade 2-6 anos: Limite inferior (72), Limite Superior (88)
    - Idade 6-18 anos: Limite inferior (71), Limite Superior (99)
    - Idade 18-59 anos Limite inferior (81,0), Limite Superior (100,1)
    - Idade 60-mais anos: Limite inferior (82,2), Limite Superior (100,7)

* **Em caso de diminuição do VCM**, pode haver um quadro de anemia por deficiência de ferro ou de origem genética.
* **O VCM alto** indica alguns tipos de anemia, alcoolismo ou alterações na medula óssea.
---

- HCM: hemoglobina globular médica é um parâmetro que indica a concentração total a hemoglobina. A análise ajuda a identificar o tipo de anemiaque a pessoa possui:
Valores de referência:
  - Masculino:
    - Idade 0-2 anos: Limite inferior (27), Limite Superior (34)
    - Idade 2-6 anos: Limite inferior (23,8), Limite Superior (34,2)
    - Idade 6-18 anos: Limite inferior (71), Limite Superior (99,6)
    - Idade 18-59 anos Limite inferior (26,9), Limite Superior (32,5)
    - Idade 60-mais anos: Limite inferior (27,6), Limite Superior (33,1)
  - Feminino:
    - Idade 0-2 anos: Limite inferior (27), Limite Superior (34)
    - Idade 2-6 anos: Limite inferior (23,8), Limite Superior (34,2)
    - Idade 6-18 anos: Limite inferior (71), Limite Superior (99,6)
    - Idade 18-59 anos Limite inferior (26,3), Limite Superior (32,3)
    - Idade 60-mais anos: Limite inferior (26,3), Limite Superior (32,6)
* **Alterações de HCM e HGM** podem ocorrer por anemia ferropriva, talassemia, consumo elevado de álcool, uso de alguns medicamentos, alterações de tireoide ou deficiência de vitamina B12 e ácido fólico. 
---

- CHCM: demonstra a concentração da hemoglobina por hemácia.
Valores de referência:
  - Masculino:
    - Idade 7 meses: Limite inferior (30), Limite Superior (36)
    - Idade 8 meses a 13 anos: Limite inferior (31), Limite Superior (36)
    - Idade 14 anos ou mais: Limite inferior (31,4), Limite Superior (36)
  - Feminino:
    - Idade 7 meses: Limite inferior (30), Limite Superior (36)
    - Idade 8 meses a 13 anos: Limite inferior (31), Limite Superior (36)
    - Idade 14 anos ou mais: Limite inferior (31,4), Limite Superior (36)
* **Valores baixos de CHCM** sugerem quadros de anemia, insuficiência cardíaca,  hipotireodismo ou interação medicamentosa. 
* **Valores altos de CHCM** estão relacionados a um consumo elevado de álcool ou problemas na glândula tireoide.
---
- PLATELET_COUNT: contagem de plaquetas, fragmentos de celúlas sanguíneas, sendo, importantes no processo de coagulção e controle de hemorragias. 
Valores de referência:
  - Masculino:
    - Idade 0-2 anos: Limite inferior (180.000), Limite Superior (658.000)
    - Idade 2-6 anos: Limite inferior (209.000), Limite Superior (455.000)
    - Idade 6-18 anos: Limite inferior (145.000), Limite Superior (455.000)
    - Idade 18-59 anos Limite inferior (128.418), Limite Superior (302.183)
    - Idade 60-mais anos: Limite inferior (128.926), Limite Superior (283.915)
  - Feminino:
    - Idade 0-2 anos: Limite inferior (180.000), Limite Superior (658.000)
    - Idade 2-6 anos: Limite inferior (209.000), Limite Superior (455.000)
    - Idade 6-18 anos: Limite inferior (145.000), Limite Superior (455.000)
    - Idade 18-59 anos Limite inferior (137.881), Limite Superior (344.744)
    - Idade 60-mais anos: Limite inferior (126.639), Limite Superior (331.474)
* **Quando as plaquetas estão reduzidas**, o risco de sangramentos fica aumentado.
* **Um aumento na quantidade de plaquetas** no sangue exige atenção para a prevenção de coágulos e trombos sanguíneos.
---
- LYMPHO: faz parte da defesa do corpo, atua contra celulas cancerígenas e infecções.
Valores referência absolutos (mm²):
- Masculino:
    - Idade 0-2 anos: Limite inferior (1.900), Limite Superior (13.500)
    - Idade 2-6 anos: Limite inferior (2.200), Limite Superior (9.400)
    - Idade 6-18 anos: Limite inferior (1.400), Limite Superior (4.300)
    - Idade 18-59 anos Limite inferior (767), Limite Superior (3.405)
    - Idade 60-mais anos: Limite inferior (582), Limite Superior (3.085)
- Feminino:
    - Idade 0-2 anos: Limite inferior (1.900), Limite Superior (13.500)
    - Idade 2-6 anos: Limite inferior (2.200), Limite Superior (9.400)
    - Idade 6-18 anos: Limite inferior (1.400), Limite Superior (4.300)
    - Idade 18-59 anos Limite inferior (825), Limite Superior (3.419)
    - Idade 60-mais anos: Limite inferior (716), Limite Superior (3.362)

- Masculino e feminino Lympho relativos(%):
  - Idade 0-18 anos: 30-60
  - Idade 18 ou mais: 20-45
* **A concentração reduzida de linfócitos** pode aparecer em casos de infecção ou desnutrição.
* **Ocorre um aumento** na quantidade destas células em casos de mononucleose infecciosa, caxumba, sarampo e algumas infecções agudas.
---

