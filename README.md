# Calculadora de espessura de isolamento térmico

Programa em Python que estima a espessura do material isolante em um sistema de refrigeração. O cálculo parte das condições do ambiente e devolve a espessura em milímetros.

### Sobre a atividade
Este projeto foi desenvolvido em **2023** para a disciplina de **Algoritmos e Estruturas de Dados I**, no **IFNMG Campus Salinas**. O exercício pedia duas implementações, uma em **C** e outra em **Python**, para calcular a espessura de isolamento necessária para evitar a condensação na superfície externa de um meio refrigerado. [Ver a versão em C](https://github.com/LucasLuidy/IFNMG-Calculadora-de-Espessura-de-Material-Isolante-em-C)

O programa usa a temperatura do ar e a umidade relativa para estimar o ponto de orvalho. Depois, combina esse valor com a temperatura do meio refrigerado, a condutividade do isolante e os coeficientes de convecção para calcular a espessura.

### Como executar
Com o **Python 3** instalado, execute os comandos abaixo. O programa usa apenas a biblioteca padrão do Python.

```js
git clone https://github.com/LucasLuidy/IFNMG-Calculadora-de-Espessura-de-Material-Isolante.git
cd IFNMG-Calculadora-de-Espessura-de-Material-Isolante
python3 main.py
```
| Dado | Unidade | Exemplo |
| --- | --- | --- |
| Temperatura de bulbo seco | °C | `25` |
| Umidade relativa do ar | % | `60` |
| Temperatura do meio refrigerado | °C | `5` |
| Condutividade térmica do isolante | W/(m·K) | `0.035` |
| Coeficiente de convecção interno | W/(m²·K) | `8` |
| Coeficiente de convecção externo | W/(m²·K) | `15` |

Para esses valores, a saída é:

```js
Espessura do material isolante: 3.81 mm
```

### Limites do cálculo
O código aplica a fórmula diretamente, sem validar as entradas. Umidade relativa de 100% ou um coeficiente de convecção igual a zero provoca divisão por zero. Dependendo dos valores informados, a fórmula também pode produzir uma espessura negativa.

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=ffdd54)](https://github.com/LucasLuidy?tab=repositories&language=python)
