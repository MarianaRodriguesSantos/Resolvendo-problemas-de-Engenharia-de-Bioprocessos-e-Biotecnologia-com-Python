# Resolvendo problemas de Engenharia de Bioprocessos e Biotecnologia com Python

Mariana Rodrigues dos Santos

Trabalho de Conclusão de Curso apresentado ao Curso de Graduação em Engenharia de Bioprocessos e Biotecnologia da Faculdade de Ciências Farmacêuticas de Araraquara, da Universidade Estadual Paulista “Júlio de Mesquita Filho”, para obtenção do grau de Engenheira de Bioprocessos e Biotecnologia.

Orientador: Prof. Dr. Marcel Otávio Cerri 

---
## Resumo

Os *softwares* computacionais tornaram muito mais simples e direta a complexa resolução de problemas de cálculo numérico, diferencial e integral aplicado à engenharia de bioprocessos e biotecnologia. Porém, a privatização destas ferramentas limitou o seu acesso, o que motivou a criação de iniciativas de *software* livre. Tais iniciativas permitiram a popularização do acesso ao conhecimento e a facilitação de resolução de problemas variados.

A linguagem de programação *Python* é uma iniciativa de *software* livre e possui várias bibliotecas voltadas para cálculo numérico, diferencial e integral. Ainda, é uma linguagem de fácil uso, o que permite que estudantes e profissionais que precisem de códigos para a resolução de problemas de cálculo possam elaborá-lo, sem precisar pagar por um programa.

Foram elaborados e publicados programas para a resolução de vários problemas comuns na vida acadêmica e profissional de engenheiros de bioprocessos e biotecnologia. Sistemas de equações lineares, aplicados em balanços de massa em destiladores e um ar condicionado, foram resolvidos empregando funções da biblioteca *NumPy*. Sistemas de equações não lineares, no contexto de uma operação com gás a altas pressões e crescimento celular de bactérias, foram solucionados pelo emprego das bibliotecas *NumPy*, *SciPy* e *Matplotlib*. As mesmas bibliotecas foram utilizadas na solução de sistemas de equações diferenciais, no caso de modelagem de um processo fermentativo. Após a publicação dos problemas e suas soluções, eles se tornaram disponíveis para consulta online por qualquer estudante ou profissional da área da engenharia.

**Palavras-chave:** Python. Programação. Engenharia. Bioprocessos. Cálculo numérico.

---
## Resultados

### **Capítulo 1** - [Sistemas de Equações Lineares](Sistemas_Equacoes_Lineares.ipynb)
**Sistema de três destiladores, proposto por Kwong (2016).**

O código deve receber, em suas primeiras linhas, o fluxo de alimentação da primeira coluna de destilação ($F$), as concentrações de cada componente na alimentação ($z_1$ a $z_4$) e as concentrações totais das correntes de saída, de topo e de fundo, dos destiladores 2 e 3 ($x_{21}$ e $y_{21}$ a $x_{34}$ e $y_{34}$). O significado e as unidades de cada variável, incógnita e dos índices empregados estão detalhados no texto explicativo que precede o código de resolução. Após a execução, o programa imprime os dados de fluxo e concentrações de cada componente, tanto na corrente de entrada como nas saídas superior e inferior de cada destilador.

**Sistema de ar condicionado, proposto por Felder *et al.* (2017).**

O programa recebe as variáveis de número de mols e quantidades relativas, necessárias para o balanço de massa de cada trecho do sistema. Os valores definidos no texto explicativo acima do código de resolução podem ser adaptados para o caso estudado. Estes valores são a quantidade, em mol, de ar que resfria o cômodo ($n_5$), as composições percentuais de ar seco e água que se inserem pelo ponto de reciclo ($m_{11}$ e $m_{21}$), que adentram o condicionador ($m_{12}$ e $m_{22}$), que são descartadas ao exterior ($m_{13}$ e $m_{23}$), e que entram no cômodo para resfriá-lo ($m_{15}$ e $m_{25}$). Com a execução, o código imprime as quantidades, em mol, de ar seco e água que entram e saem de cada trecho do sistema, ou seja, o condicionador, o cômodo, o exterior e o ponto de reciclagem.

### **Capítulo 2** - [Sistemas de Equações Não Lineares](Sistemas_Equacoes_Nao_Lineares.ipynb)
**Operação com gás a altas pressões, proposto por Kwong (2016).**

O código deve receber, nas primeiras linhas, as características de temperatura e pressão críticas do gás de estudo, e as características de temperatura e pressão do processo. Ao final da execução é impresso o volume molar do gás nas condições estabelecidas.

**Crescimento microbiano descrito por modelo publicado por Huang (2013).**

É necessário inserir no programa, em suas primeiras linhas, os valores característicos do microrganismo estudado e das condições de cultivo estabelecidas. São empregados a taxa de crescimento específica do microrganismo ($\mu_{máx}$), o coeficiente de transição da fase lag e sua duração ($\alpha$ e $\lambda$), além das concentrações inicial e máxima de células ao longo do cultivo ($Y_0$ e $Y_{máx}$). Após executar o código, é impresso um gráfico que mostra a concentração celular no meio em função do tempo de crescimento.

### **Capítulo 3** - [Sistemas de Equações Diferenciais Ordinárias](Sistemas_Equacoes_Diferenciais_Ordinarias.ipynb)
**Concentração de componentes em processo fermentativo, a partir de cinética de Monod e modelo de Luedeking e Piret.**

Nas linhas iniciais do programa é preciso definir as constantes do crescimento microbiano nas condições estabelecidas. São necessários a taxa de crescimento específica do microrganismo ($\mu_{máx}$), a constante de saturação ($K_S$), o periodo de crescimento ($tf$, no código), a concentração de substrato no início do crescimento ($S_0$) e na alimentação ($S_i$), a concentração de produto no início ($P_0$) e na alimentação ($P_i$), o volume inicial de cultivo ($V_0$), a vazão de alimentação ($Q$), o coeficiente estequiométrico de conversão de substrato em biomassa ($Y_{XS}$) e as constantes de Luedeking e Piret ($\alpha$ e $\beta$). A execução resulta na impressão de um gráfico que mostra a variação das concentrações de substrato, produto e células no meio de cultivo ao longo do tempo.

## Execução dos códigos

Todos os documentos aqui disponíveis foram elaborados no *Google Colab*, utilizando o sistema *Markdown* de formatação de textos e a linguagem de programação *Python*. Portanto, os programas podem ser baixados aqui no *GitHub* e executados pelo [*site* do *Google Colab*](https://colab.research.google.com/).

---
## Referências Bibliográficas

### Referências dos problemas

1. FELDER, Richard M. *et al*. **Princípios elementares dos processos químicos**. 4. ed. Rio de Janeiro: Livros Técnicos e Científicos Editora, 2017. ISBN 978-85-216-3492-8.

2. HUANG, Lihan. Optimization of a new mathematical model for bacterial growth. **Food Control**, v. 32, n. 1, p. 283-288, jul. 2013. Disponível em: <https://doi.org/10.1016/j.foodcont.2012.11.019>. Acesso em: 19 abr. 2024.

3. KWONG, Wu Hong. **Resolvendo Problemas de Engenharia Química com Software Livre Scilab**. São Carlos, SP: EdUFSCar, 2016. 667 p. ISBN 978-85-7600-425-7.

4. MATPLOTLIB. **Matplotlib documentation**: API Reference. Version 3.8.4. 2023. Documentação, disponível online, de biblioteca para uso em linguagem de programação Python. Disponível em: <https://matplotlib.org/stable/api/index.html>. Acesso em: 18 abr. 2024.

5. NUMPY. **NumPy Documentation**: Linear Algebra (numpy.linalg). Version 1.24. 2022. Documentação, disponível online, de biblioteca para uso em linguagem de programação Python. Disponível em: <https://numpy.org/doc/stable/reference/routines.linalg.html#module-numpy.linalg>. Acesso em: 11 abr. 2023.

6. SCIPY. **SciPy Documentation**: User guide. Version 1.10.1. 2023. Documentação, disponível online, de biblioteca para uso em linguagem de programação Python. Disponível em: <https://docs.scipy.org/doc/scipy/tutorial/index.html>. Acesso em: 28 mai. 2023.


### Fundamentação teórica

1. AGUILAR, Luis Joyanes. Introdução à ciência da computação e à programação. *In:* AGUILAR, Luis Joyanes. **Programação em C++**: Algoritmos, estruturas de dados e objetos. 2. ed. Porto Alegre, RS: AMGH, 2008. cap. 1, p. 3-41. ISBN 978-85-8055-026-9.

2. ANTON, Howard; RORRES, Chris. **Álgebra Linear com Aplicações**. 10. ed. Porto Alegre, RS: Bookman, 2012. 768 p. ISBN 978-85-407-0169-4.

3. FERNANDES, Daniela Barude. **Cálculo Numérico**. 1. ed. São Paulo: Pearson, 2015. ISBN 978-85-430-1712-9.

4. GITHUB. Git Guide. *In:* GITHUB. **GitHub**. 2024. Website oficial da plataforma de hospedagem de arquivos e códigos. Disponível em: <https://github.com/git-guides>. Acesso em: 23 abr. 2024.

5. GNU. Filosofia do Projeto GNU. *In:* GNU. **O Sistema Operacional GNU**. 2022. Tradução do website original da organização GNU. Disponível em: <https://www.gnu.org/philosophy/philosophy.html>. Acesso em: 12 mar. 2024.

6. GOOGLE. Google Colaboratory. *In:* GOOGLE. **Google Colab**. 2024. Website oficial do serviço Google Colab. Disponível em: <https://colab.google/>. Acesso em: 22 abr. 2024.

7. HARRIS, Frank E. Ordinary Differential Equations. *In:* HARRIS, Frank E. **Mathematics for Physical Science and Engineering**: Symbolic Computing Applications in Maple and Mathematica. 1. ed. Academic Press, 2014. cap. 10, p. 349-396. ISBN 978-01-2801-000-6. Disponível em: <https://doi.org/10.1016/B978-0-12-801000-6.00010-9>. Acesso em: 26 fev. 2024.

8. JARLETTI, Celina. **Cálculo Numérico**. 1. ed. Curitiba, PR: InterSaberes, 2018. ISBN 978-85-5972-661-9.

9. PROJECT JUPYTER. About Us: Project Jupyter’s origins and governance. *In:* PROJECT JUPYTER. Jupyter Notebook. 2024. Seção “Sobre” do projeto **Jupyter Notebook**. Disponível em: <https://jupyter.org/about>. Acesso em: 22 abr. 2024.

10. SPERANDIO, Décio; SILVA, Luiz Henry Monken. **Cálculo numérico e programação matemática**: aplicações. 1. ed. Curitiba, PR: InterSaberes, 2022. ISBN 978-65-5517-332-1.

11. SURENDHIRAN, D. *et al*. Kinetic modeling of microalgal growth and lipid synthesis for biodiesel production. **3 Biotech**, v. 5, p. 663-669, out. 2015. Disponível em: <https://doi.org/10.1007/s13205-014-0264-3>. Acesso em: 15 abr. 2024.

12. MOZILLA. Manifesto Mozilla: Nossos 10 princípios. *In:* MOZILLA. **Mozilla website**. 2024. Manifesto da organização responsável pela administração do navegador Mozilla Firefox. Disponível em: <https://www.mozilla.org/pt-BR/about/manifesto/>. Acesso em: 12 mar. 2024.

13. PYTHON SOFTWARE FOUNDATION. About. *In:* PYTHON SOFTWARE FOUNDATION. **Python**. 2024. Seção sobre a linguagem de programação Python no seu website oficial. Disponível em: <https://www.python.org/about/>. Acesso em: 13 mar. 2024.

14. RUGGIERO, Márcia A. Gomes; LOPES, Vera Lúcia da Rocha. **Cálculo Numérico**: Aspectos teóricos e computacionais. 2. ed. São Paulo: Pearson, 1996. ISBN 978-85-346-0204-4.
